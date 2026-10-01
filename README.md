<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>HYPACK XYZ Z Value Adjuster</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            background: #f2f4f7;
            margin: 0;
            padding: 30px;
        }

        .container {
            max-width: 750px;
            margin: auto;
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 2px 12px rgba(0,0,0,0.12);
        }

        h1 {
            margin-top: 0;
            color: #1f2937;
        }

        .description {
            color: #555;
            line-height: 1.5;
        }

        label {
            display: block;
            margin-top: 20px;
            margin-bottom: 7px;
            font-weight: bold;
        }

        input[type="file"],
        input[type="number"] {
            width: 100%;
            box-sizing: border-box;
            padding: 12px;
            font-size: 16px;
            border: 1px solid #bbb;
            border-radius: 6px;
        }

        button {
            margin-top: 25px;
            padding: 13px 22px;
            font-size: 16px;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }

        #processBtn {
            background: #2563eb;
            color: white;
        }

        #downloadBtn {
            background: #16a34a;
            color: white;
            display: none;
        }

        button:hover {
            opacity: 0.9;
        }

        .info {
            margin-top: 20px;
            padding: 15px;
            background: #eef6ff;
            border-left: 4px solid #2563eb;
        }

        .result {
            margin-top: 20px;
            padding: 15px;
            background: #f5f5f5;
            border-radius: 6px;
            white-space: pre-wrap;
            font-family: monospace;
            max-height: 220px;
            overflow-y: auto;
        }

        .example {
            background: #fafafa;
            padding: 15px;
            border-radius: 6px;
            margin-top: 20px;
            font-family: monospace;
        }
    </style>
</head>

<body>

<div class="container">

    <h1>HYPACK XYZ Z Value Adjuster</h1>

    <p class="description">
        Adjust the Z values in a HYPACK XYZ text file.
        X and Y values remain unchanged. Only the third column (Z)
        is increased or decreased by the value you enter.
    </p>

    <div class="example">
        Original:<br>
        979390.72 179494.63 37.47<br><br>

        Adjustment: +1.50<br><br>

        Result:<br>
        979390.72 179494.63 38.97
    </div>

    <label for="fileInput">Select HYPACK XYZ / TXT file</label>

    <input
        type="file"
        id="fileInput"
        accept=".txt,.xyz"
    >

    <label for="adjustment">Z Adjustment</label>

    <input
        type="number"
        id="adjustment"
        value="0"
        step="0.01"
        placeholder="Example: 1.5 or -2.2"
    >

    <div class="info">
        <strong>Examples:</strong><br>
        Enter <strong>1.5</strong> → adds 1.50 to every Z value<br>
        Enter <strong>-2.2</strong> → subtracts 2.20 from every Z value
    </div>

    <button id="processBtn">
        Process XYZ File
    </button>

    <button id="downloadBtn">
        Download Corrected XYZ File
    </button>

    <div id="status"></div>

    <div id="result" class="result"></div>

</div>


<script>

let outputText = "";
let originalFileName = "";


document.getElementById("processBtn").addEventListener("click", function () {

    const fileInput = document.getElementById("fileInput");
    const adjustmentInput = document.getElementById("adjustment");

    const status = document.getElementById("status");
    const result = document.getElementById("result");
    const downloadBtn = document.getElementById("downloadBtn");

    if (!fileInput.files.length) {
        alert("Please select an XYZ or TXT file.");
        return;
    }

    const adjustment = Number(adjustmentInput.value);

    if (!Number.isFinite(adjustment)) {
        alert("Please enter a valid adjustment value.");
        return;
    }

    const file = fileInput.files[0];

    originalFileName = file.name;

    const reader = new FileReader();

    reader.onload = function (event) {

        const text = event.target.result;

        const lines = text.split(/\r?\n/);

        let processedLines = [];
        let validPoints = 0;
        let unchangedLines = 0;

        for (let line of lines) {

            // Keep blank lines unchanged
            if (line.trim() === "") {
                processedLines.push(line);
                continue;
            }

            /*
             * Split the line by whitespace.
             *
             * Expected:
             * X Y Z
             */
            const parts = line.trim().split(/\s+/);

            if (parts.length >= 3) {

                const x = parts[0];
                const y = parts[1];
                const z = Number(parts[2]);

                if (
                    Number.isFinite(Number(x)) &&
                    Number.isFinite(Number(y)) &&
                    Number.isFinite(z)
                ) {

                    const newZ = z + adjustment;

                    /*
                     * Output Z with two decimal places.
                     */
                    processedLines.push(
                        x + " " +
                        y + " " +
                        newZ.toFixed(2)
                    );

                    validPoints++;

                } else {

                    processedLines.push(line);
                    unchangedLines++;
                }

            } else {

                // Keep lines that don't contain XYZ unchanged
                processedLines.push(line);
                unchangedLines++;
            }
        }

        outputText = processedLines.join("\n");

        status.innerHTML =
            "<div class='info'>" +
            "<strong>Processing complete.</strong><br>" +
            "Points processed: " + validPoints.toLocaleString() + "<br>" +
            "Lines unchanged: " + unchangedLines.toLocaleString() +
            "</div>";

        /*
         * Show first 10 processed lines
         */
        result.textContent =
            processedLines.slice(0, 10).join("\n");

        downloadBtn.style.display = "inline-block";
    };

    reader.readAsText(file);
});


document.getElementById("downloadBtn").addEventListener("click", function () {

    if (!outputText) {
        alert("Please process a file first.");
        return;
    }

    /*
     * Create downloadable text file
     */
    const blob = new Blob(
        [outputText],
        { type: "text/plain;charset=utf-8" }
    );

    const url = URL.createObjectURL(blob);

    const link = document.createElement("a");

    link.href = url;

    /*
     * Create output filename
     */
    const baseName = originalFileName.replace(/\.[^/.]+$/, "");

    link.download = baseName + "_Z_ADJUSTED.txt";

    document.body.appendChild(link);

    link.click();

    document.body.removeChild(link);

    URL.revokeObjectURL(url);
});

</script>

</body>
</html>
