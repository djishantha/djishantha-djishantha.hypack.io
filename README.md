<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FREE HYPACK CAD Tools</title>
<style>
:root{--ink:#0b4f7a;--sea:#0a6ea5;--sea-d:#085888;--paper:#eef6fb;--line:#cfe1ec;--mut:#546e80;
      --ok:#0a6b43;--okbg:#e6f5ec;--bad:#a32017;--badbg:#fdeceb;--tint:#e1f1fa}
*{box-sizing:border-box}
body{margin:0;background:var(--paper);color:#14303f;font:16px/1.5 "Segoe UI",system-ui,-apple-system,Roboto,Arial,sans-serif}
.wrap{max-width:760px;margin:0 auto}
.top{position:relative;background:linear-gradient(180deg,#3fa6df 0%,#8fd2f1 60%,#cfeefb 100%);overflow:hidden}
.top .sky{position:absolute;inset:0;width:100%;height:100%;pointer-events:none}
.top .wrap{position:relative;padding:26px 20px 6px}
h1{margin:0;font-size:1.75rem;font-weight:800;color:#06385a;letter-spacing:.3px}
.surf{position:relative;display:block;width:100%;height:46px;margin-bottom:-1px}
.sea{position:relative;background:#0a6ea5}
.sea .wrap{padding:0 20px}
.tabs{display:flex;gap:4px;overflow-x:auto;padding-top:2px}
.tab-button{flex:0 0 auto;margin:0;padding:11px 18px;border:0;border-radius:8px 8px 0 0;background:transparent;color:#dff2fb;font:600 15px/1.2 inherit;cursor:pointer}
.tab-button:hover{color:#fff;background:rgba(255,255,255,.12)}
.tab-button.active{background:var(--paper);color:var(--ink)}
main{max-width:760px;margin:0 auto;padding:22px 20px 48px}
.tab-content{display:none}
.tab-content.active{display:block}
.section{background:#fff;border:1px solid var(--line);border-radius:10px;padding:22px;margin-bottom:16px}
.section h2{margin:0 0 2px;font-size:1.15rem;color:var(--ink)}
.description{margin:0;color:var(--mut);font-size:.92rem}
label{display:block;margin:18px 0 6px;font-weight:600;font-size:.9rem;color:#2c4252}
input[type=file],input[type=number],select{width:100%;padding:10px 12px;font:inherit;font-size:15px;color:inherit;background:#fff;border:1px solid var(--line);border-radius:8px}
input[type=file]::file-selector-button{margin-right:12px;padding:7px 14px;border:0;border-radius:6px;background:var(--ink);color:#fff;font:600 14px inherit;cursor:pointer}
.hint{margin:8px 0 0;color:var(--mut);font-size:.86rem}
.file-name{margin-top:6px;color:var(--mut);font-size:.86rem}
.check{display:flex;align-items:center;gap:10px;margin-top:18px;font-weight:600;cursor:pointer}
.check input{width:18px;height:18px;accent-color:var(--sea)}
.formula{margin-top:18px;padding:10px 14px;border-radius:8px;background:var(--tint);color:var(--ink);font:600 15px Consolas,Menlo,monospace}
button{font:inherit;font-weight:600;padding:11px 20px;border:1px solid transparent;border-radius:8px;cursor:pointer}
button:disabled{opacity:.45;cursor:not-allowed}
.actionRow{display:flex;gap:10px;flex-wrap:wrap;margin-top:20px}
.processBtn{background:var(--sea);color:#fff}
.processBtn:hover:not(:disabled){background:var(--sea-d)}
.downloadBtn{display:none;background:var(--ink);color:#fff}
.downloadBtn:hover{opacity:.88}
.clearBtn{background:transparent;color:var(--mut);border-color:var(--line)}
.clearBtn:hover{color:var(--ink);border-color:var(--mut)}
.info,.success,.error{margin-top:16px;padding:12px 14px;border-radius:8px}
.info{background:var(--tint)}
.success{background:var(--okbg);color:var(--ok)}
.error{background:var(--badbg);color:var(--bad)}
.result{margin-top:16px;padding:12px 14px;background:var(--paper);border:1px solid var(--line);border-radius:8px;font:13px/1.5 Consolas,Menlo,monospace;white-space:pre-wrap;max-height:260px;overflow:auto}
.result:empty{display:none}
#vdatumProgressContainer{display:none;margin-top:16px}
#vdatumProgressBar{width:100%;height:14px;accent-color:var(--sea)}
#vdatumProgressText{margin-top:4px;text-align:center;font-weight:600;font-size:.9rem}
#vdatumDownloadSection{display:none;margin-top:16px;padding:16px;border-radius:8px;background:var(--tint)}
#vdatumDownloadSection h3{margin:0 0 4px;font-size:1rem}
#vdatumDownloadButton{margin-top:12px;background:var(--ink);color:#fff}
#cvPreview{overflow-x:auto}
#cvPreview h3{margin:18px 0 6px;font-size:.95rem;color:var(--ink)}
#cvPreview table{width:100%;border-collapse:collapse;font-size:13px}
#cvPreview th,#cvPreview td{padding:6px 8px;border-bottom:1px solid var(--line);text-align:right}
#cvPreview th{color:var(--mut);font-weight:600}
.footer{display:flex;justify-content:flex-end;margin-top:4px}
button:focus-visible,select:focus-visible,input:focus-visible{outline:3px solid var(--sea);outline-offset:2px}
@media(max-width:560px){.tab-button{padding:10px 12px;font-size:14px}.section{padding:16px}}
</style>
</head>
<body>
<header class="top">
  <svg class="sky" viewBox="0 0 800 160" preserveAspectRatio="xMaxYMin slice" aria-hidden="true">
    <g fill="#fff" opacity=".85">
      <ellipse cx="600" cy="38" rx="46" ry="13"/><ellipse cx="632" cy="30" rx="30" ry="14"/><ellipse cx="572" cy="34" rx="26" ry="10"/>
      <ellipse cx="730" cy="78" rx="34" ry="9"/><ellipse cx="752" cy="72" rx="20" ry="10"/>
      <ellipse cx="430" cy="22" rx="30" ry="8" opacity=".7"/>
    </g>
    <circle cx="690" cy="26" r="16" fill="#fff6c9" opacity=".9"/>
  </svg>
  <div class="wrap"><h1>FREE HYPACK CAD Tools</h1></div>
  <svg class="surf" viewBox="0 0 1440 46" preserveAspectRatio="none" aria-hidden="true">
    <path d="M0 22 C120 6 240 6 360 22 S600 38 720 22 S960 6 1080 22 S1320 38 1440 22 V46 H0 Z" fill="#5db9e6" opacity=".75"/>
    <path d="M0 30 C140 14 260 14 400 30 S640 46 780 30 S1020 14 1160 30 S1340 42 1440 30 V46 H0 Z" fill="#0a6ea5"/>
  </svg>
  <div class="sea"><div class="wrap">
    <nav class="tabs">
      <button class="tab-button active" onclick="openTab('vdatumTab', this)">VDATUM</button>
      <button class="tab-button" onclick="openTab('zAdjustTab', this)">Z Adjust</button>
      <button class="tab-button" onclick="openTab('cvTab', this)">Convert Grid</button>
      <button class="tab-button" onclick="openTab('mtxChnTab', this)">Extract XYZ</button>
    </nav>
  </div></div>
</header>

<main>

<div id="vdatumTab" class="tab-content active">
  <div class="section">
    <h2>VDATUM Z Adjustment</h2>
    <p class="description">Matches each survey point to the nearest VDATUM point.</p>
    <label for="vdatumFile">VDATUM MLLW XYZ file</label>
    <input type="file" id="vdatumFile" accept=".xyz,.txt">
    <div id="vdatumName" class="file-name">No VDATUM file selected</div>
    <label for="surveyFile">Survey XYZ file</label>
    <input type="file" id="surveyFile" accept=".xyz,.txt">
    <div id="surveyName" class="file-name">No survey file selected</div>
    <label class="check"><input type="checkbox" id="vdatumRound"> Round X Y to 2 decimals, Z to 1 decimal</label>
    <div class="formula">New Z = Survey Z + VDATUM Z</div>
    <div class="actionRow">
      <button id="vdatumProcessButton" class="processBtn">Process</button>
      <button id="vdatumRefreshButton" class="clearBtn">Clear</button>
    </div>
    <div id="vdatumProgressContainer">
      <progress id="vdatumProgressBar" value="0" max="100"></progress>
      <div id="vdatumProgressText">0%</div>
    </div>
    <div id="vdatumStatus" class="result"></div>
    <div id="vdatumDownloadSection">
      <h3>Output ready</h3>
      <div id="vdatumOutputFileName" class="file-name"></div>
      <button id="vdatumDownloadButton">Download XYZ</button>
    </div>
  </div>
</div>

<div id="zAdjustTab" class="tab-content">
  <div class="section">
    <h2>Z Adjust / Invert</h2>
    <p class="description">Shift, invert and round Z values.</p>
    <label for="zAdjustFile">XYZ / TXT file</label>
    <input type="file" id="zAdjustFile" accept=".txt,.xyz">
    <label for="zAdjustment">Z adjustment</label>
    <input type="number" id="zAdjustment" value="0" step="0.01" placeholder="1.5 or -2.2">
    <p class="hint">Positive adds, negative subtracts.</p>
    <label class="check"><input type="checkbox" id="invertZAdjust"> Invert Z values</label>
    <label class="check"><input type="checkbox" id="zRound" checked> Round X Y to 2 decimals, Z to 1 decimal</label>
    <div class="actionRow">
      <button id="zProcessBtn" class="processBtn">Process</button>
      <button id="zDownloadBtn" class="downloadBtn">Download XYZ</button>
    </div>
    <div id="zStatus"></div>
    <div id="zResult" class="result"></div>
  </div>
</div>

<div id="cvTab" class="tab-content">
  <div class="section">
    <h2>Convert Grid</h2>
    <p class="description">NAD83, US survey feet. Z is unchanged.</p>
    <label for="cvDir">Conversion</label>
    <select id="cvDir">
      <option value="NJ>NYLI">NJ 2900 &rarr; NY Long Island 3104</option>
      <option value="NYLI>NJ">NY Long Island 3104 &rarr; NJ 2900</option>
      <option value="NJ>NYE">NJ 2900 &rarr; NY East 3101</option>
      <option value="NYE>NJ">NY East 3101 &rarr; NJ 2900</option>
      <option value="NYE>NYLI">NY East 3101 &rarr; NY Long Island 3104</option>
      <option value="NYLI>NYE">NY Long Island 3104 &rarr; NY East 3101</option>
    </select>
    <p id="cvNote" class="hint" style="display:none">Same projection, so X Y stay the same.</p>
    <label for="cvFile">File</label>
    <input type="file" id="cvFile" accept=".txt,.xyz,.csv,.pts,.dat">
    <label class="check"><input type="checkbox" id="cvRound"> Round X Y to 2 decimals, Z to 1 decimal</label>
    <p class="hint">Columns are detected automatically. Projection only; no datum shift applied.</p>
    <div class="actionRow">
      <button id="cvConvertBtn" class="processBtn" disabled>Convert</button>
      <button id="cvDownloadBtn" class="downloadBtn">Download</button>
    </div>
    <div id="cvStatus"></div>
    <div id="cvPreview"></div>
  </div>
</div>

<div id="mtxChnTab" class="tab-content">
  <div class="section">
    <h2>MTX &rarr; Four Corner XYZ</h2>
    <p class="description">Outside corners of an MTX grid.</p>
    <label for="mtxFile">MTX file</label>
    <input type="file" id="mtxFile" accept=".mtx,.txt">
    <label for="mtxZ">Corner Z</label>
    <input type="number" id="mtxZ" value="0" step="0.1">
    <div class="actionRow">
      <button id="mtxProcessBtn" class="processBtn">Process</button>
      <button id="mtxDownloadBtn" class="downloadBtn">Download XYZ</button>
      <button id="mtxClearBtn" class="clearBtn">Clear</button>
    </div>
    <div id="mtxStatus"></div>
    <div id="mtxResult" class="result"></div>
  </div>

  <div class="section">
    <h2>CHN &rarr; XYZ Nodes</h2>
    <p class="description">Channel nodes as X Y Z.</p>
    <label for="chnFile">CHN file</label>
    <input type="file" id="chnFile" accept=".chn,.txt">
    <div class="actionRow">
      <button id="chnProcessBtn" class="processBtn">Process</button>
      <button id="chnDownloadBtn" class="downloadBtn">Download XYZ</button>
      <button id="chnClearBtn" class="clearBtn">Clear</button>
    </div>
    <div id="chnStatus"></div>
    <div id="chnResult" class="result"></div>
  </div>
</div>

<div class="footer"><button id="clearAllBtn" class="clearBtn">Clear all</button></div>

</main>

<script>

function roundHalfUp(v, d) {
    const f = Math.pow(10, d);
    return (Math.sign(v) * Math.round(Math.abs(v) * f + 1e-9) / f).toFixed(d);
}



/* ============================================================
   TAB CONTROL
============================================================ */

function openTab(tabId, button) {

    document
        .querySelectorAll(".tab-content")
        .forEach(function(tab) {
            tab.classList.remove("active");
        });

    document
        .querySelectorAll(".tab-button")
        .forEach(function(btn) {
            btn.classList.remove("active");
        });

    document
        .getElementById(tabId)
        .classList.add("active");

    button.classList.add("active");
}




/* ============================================================
   GLOBAL VARIABLES
============================================================ */

let mtxOutputText = "";
let mtxOriginalFileName = "";

let chnOutputText = "";
let chnOriginalFileName = "";



/* ============================================================
   MTX PROCESS
============================================================ */

document
.getElementById("mtxProcessBtn")
.addEventListener("click", function() {


    const fileInput =
        document.getElementById("mtxFile");


    const zInput =
        document.getElementById("mtxZ");


    const status =
        document.getElementById("mtxStatus");


    const result =
        document.getElementById("mtxResult");


    const downloadBtn =
        document.getElementById("mtxDownloadBtn");


    if (!fileInput.files.length) {

        alert("Please select an MTX file.");

        return;

    }


    const zValue =
        Number(zInput.value);


    if (!Number.isFinite(zValue)) {

        alert("Please enter a valid Z value.");

        return;

    }


    const file =
        fileInput.files[0];


    mtxOriginalFileName =
        file.name;


    const reader =
        new FileReader();


    reader.onload =
        function(event) {


            const text =
                event.target.result;


            const values =
                extractMTXValues(text);


            if (values.length < 7) {

                status.innerHTML =
                    "<div class='error'>" +

                    "<strong>Error:</strong><br>" +

                    "Could not find the required " +
                    "7 MTX values.<br>" +

                    "Values found: " +
                    values.length +

                    "</div>";

                downloadBtn.style.display =
                    "none";

                return;

            }


            /*
             * MTX structure
             *
             * 0 = X
             * 1 = Y
             * 2 = Width
             * 3 = First Leg / Length
             * 4 = Grid X
             * 5 = Grid Y
             * 6 = Bearing
             */


            const x0 =
                values[0];

            const y0 =
                values[1];

            const width =
                values[2];

            const length =
                values[3];

            const bearingDeg =
                values[6];


            /*
             * Calculate four corners.
             */

            const corners =
                calculateCorners(
                    x0,
                    y0,
                    width,
                    length,
                    bearingDeg,
                    zValue
                );


            /*
             * Create XYZ output.
             */

            mtxOutputText =
                corners
                .map(function(point) {

                    return (
                        point.x.toFixed(3) +
                        " " +
                        point.y.toFixed(3) +
                        " " +
                        point.z.toFixed(1)
                    );

                })
                .join("\n");


            /*
             * Status.
             */

            status.innerHTML =
                "<div class='success'>" +

                "<strong>MTX processing complete.</strong>" +

                "<br><br>" +

                "X: " +
                x0 +

                "<br>" +

                "Y: " +
                y0 +

                "<br>" +

                "Width: " +
                width +

                "<br>" +

                "First Leg: " +
                length +

                "<br>" +

                "Bearing from North: " +
                bearingDeg +
                "°" +

                "<br>" +

                "Z: " +
                zValue +

                "</div>";


            /*
             * Preview.
             */

            result.textContent =
                mtxOutputText;


            /*
             * Show download.
             */

            downloadBtn.style.display =
                "inline-block";

        };


    reader.readAsText(file);

});



/* ============================================================
   EXTRACT MTX VALUES
============================================================ */

function extractMTXValues(text) {


    const lines =
        text.split(/\r?\n/);


    let values = [];


    for (let line of lines) {


        line =
            line.trim();


        if (line === "") {

            continue;

        }


        /*
         * Remove comments.
         */

        line =
            line.replace(
                /#.*$/,
                ""
            );


        line =
            line.replace(
                /\/\/.*$/,
                ""
            );


        if (line.trim() === "") {

            continue;

        }


        /*
         * Find numbers.
         */

        const matches =
            line.match(
                /[-+]?(?:\d+(?:\.\d*)?|\.\d+)(?:[Ee][-+]?\d+)?/g
            );


        if (
            matches &&
            matches.length > 0
        ) {

            const value =
                Number(matches[0]);


            if (
                Number.isFinite(value)
            ) {

                values.push(value);

            }

        }

    }


    return values;

}



/* ============================================================
   CALCULATE FOUR CORNERS
============================================================ */

function calculateCorners(
    x0,
    y0,
    width,
    length,
    bearingDeg,
    z
) {


    /*
     * Bearing is clockwise from North.
     *
     * 0°   = North
     * 90°  = East
     * 180° = South
     * 270° = West
     */


    const bearing =
        bearingDeg *
        Math.PI /
        180;


    /*
     * First leg direction.
     */

    const ux =
        Math.sin(bearing);

    const uy =
        Math.cos(bearing);


    /*
     * Perpendicular direction.
     *
     * Clockwise numbering.
     */

    const vx =
        Math.cos(bearing);

    const vy =
        -Math.sin(bearing);


    /*
     * Corner 1
     */

    const p1 = {

        x: x0,
        y: y0,
        z: z

    };


    /*
     * Corner 2
     */

    const p2 = {

        x:
            x0 +
            length * ux,

        y:
            y0 +
            length * uy,

        z: z

    };


    /*
     * Corner 3
     */

    const p3 = {

        x:
            x0 +
            length * ux +
            width * vx,

        y:
            y0 +
            length * uy +
            width * vy,

        z: z

    };


    /*
     * Corner 4
     */

    const p4 = {

        x:
            x0 +
            width * vx,

        y:
            y0 +
            width * vy,

        z: z

    };


    return [
        p1,
        p2,
        p3,
        p4
    ];

}



/* ============================================================
   MTX DOWNLOAD
============================================================ */

document
.getElementById("mtxDownloadBtn")
.addEventListener("click", function() {


    if (!mtxOutputText) {

        alert(
            "Please process an MTX file first."
        );

        return;

    }


    const blob =
        new Blob(
            [mtxOutputText],
            {
                type:
                    "text/plain;charset=utf-8"
            }
        );


    const url =
        URL.createObjectURL(blob);


    const link =
        document.createElement("a");


    link.href =
        url;


    const baseName =
        mtxOriginalFileName
        .replace(
            /\.[^/.]+$/,
            ""
        );


    link.download =
        baseName +
        "_four_corners.xyz";


    document.body.appendChild(link);

    link.click();

    document.body.removeChild(link);


    URL.revokeObjectURL(url);

});



/* ============================================================
   MTX CLEAR
============================================================ */

document
.getElementById("mtxClearBtn")
.addEventListener("click", function() {


    document.getElementById(
        "mtxFile"
    ).value = "";


    document.getElementById(
        "mtxZ"
    ).value = "0";


    document.getElementById(
        "mtxStatus"
    ).innerHTML = "";


    document.getElementById(
        "mtxResult"
    ).textContent = "";


    document.getElementById(
        "mtxDownloadBtn"
    ).style.display = "none";


    mtxOutputText = "";

    mtxOriginalFileName = "";

});



/* ============================================================
   CHN PROCESS
============================================================ */

document
.getElementById("chnProcessBtn")
.addEventListener("click", function() {


    const fileInput =
        document.getElementById("chnFile");


    const status =
        document.getElementById("chnStatus");


    const result =
        document.getElementById("chnResult");


    const downloadBtn =
        document.getElementById(
            "chnDownloadBtn"
        );


    if (!fileInput.files.length) {

        alert("Please select a CHN file.");

        return;

    }


    const file =
        fileInput.files[0];


    chnOriginalFileName =
        file.name;


    const reader =
        new FileReader();


    reader.onload =
        function(event) {


            const text =
                event.target.result;


            const points =
                extractCHNNodes(text);


            if (
                points.length === 0
            ) {

                status.innerHTML =
                    "<div class='error'>" +

                    "<strong>Error:</strong><br>" +

                    "No CHN nodes were found." +

                    "<br><br>" +

                    "The CHN file structure may be different " +
                    "from the expected HYPACK node format." +

                    "</div>";


                result.textContent = "";

                downloadBtn.style.display =
                    "none";

                return;

            }


            /*
             * Create XYZ output.
             */

            chnOutputText =
                points
                .map(function(point) {

                    return (
                        point.x.toFixed(3) +
                        " " +
                        point.y.toFixed(3) +
                        " " +
                        point.z.toFixed(3)
                    );

                })
                .join("\n");


            /*
             * Status.
             */

            status.innerHTML =
                "<div class='success'>" +

                "<strong>CHN processing complete.</strong>" +

                "<br><br>" +

                "Nodes extracted: " +

                points.length.toLocaleString() +

                "</div>";


            /*
             * Preview first 20 nodes.
             */

            result.textContent =
                points
                .slice(0, 20)
                .map(function(point) {

                    return (
                        point.x.toFixed(3) +
                        " " +
                        point.y.toFixed(3) +
                        " " +
                        point.z.toFixed(3)
                    );

                })
                .join("\n");


            if (
                points.length > 20
            ) {

                result.textContent +=
                    "\n\n... " +
                    (
                        points.length - 20
                    ).toLocaleString() +
                    " more points ...";

            }


            /*
             * Show download.
             */

            downloadBtn.style.display =
                "inline-block";

        };


    reader.readAsText(file);

});



/* ============================================================
   EXTRACT CHN NODES
============================================================ */

function extractCHNNodes(text) {

    const lines = text.split(/\r?\n/);

    let points = [];
    const seen = new Set();

    /*
     * HYPACK CHN structure:
     *
     * NODES <number of nodes>
     * X Y Z NodeNumber
     * X Y Z NodeNumber
     * ...
     *
     * The node section ends when FACES, SEGMENTS,
     * LABELS, ZONES, ELEVATION, or another section
     * begins.
     */

    let inNodesSection = false;
    let expectedNodes = 0;

    for (let line of lines) {

        line = line.trim();

        if (line === "") {
            continue;
        }

        /*
         * Start of NODES section.
         */

        const nodesMatch = line.match(/^NODES\s+(\d+)/i);

        if (nodesMatch) {

            inNodesSection = true;
            expectedNodes = Number(nodesMatch[1]);

            continue;
        }

        /*
         * Stop when another CHN section begins.
         */

        if (
            /^(FACES|SEGMENTS|LABELS|ZONES|ELEVATION|\[Settings\])/i.test(line)
        ) {

            if (inNodesSection) {
                break;
            }

            continue;
        }

        if (!inNodesSection) {
            continue;
        }

        /*
         * Convert commas and tabs to spaces.
         */

        const parts = line
            .replace(/,/g, " ")
            .trim()
            .split(/\s+/);

        if (parts.length < 4) {
            continue;
        }

        /*
         * Actual HYPACK CHN node format:
         *
         * X Y Z NodeNumber
         */

        const x = Number(parts[0]);
        const y = Number(parts[1]);
        const z = Number(parts[2]);
        const node = Number(parts[3]);

        /*
         * All four values must be numeric.
         */

        if (
            !Number.isFinite(x) ||
            !Number.isFinite(y) ||
            !Number.isFinite(z) ||
            !Number.isFinite(node)
        ) {
            continue;
        }

        /*
         * Node number must be an integer.
         */

        if (
            Math.abs(node - Math.round(node)) > 0.000001
        ) {
            continue;
        }

        /*
         * State Plane coordinate check.
         */

        if (
            Math.abs(x) < 100000 ||
            Math.abs(y) < 10000
        ) {
            continue;
        }

        /*
         * Prevent duplicate XYZ points.
         */

        const key =
            x.toFixed(6) +
            "|" +
            y.toFixed(6) +
            "|" +
            z.toFixed(6);

        if (seen.has(key)) {
            continue;
        }

        seen.add(key);

        /*
         * Save only X Y Z.
         */

        points.push({
            x: x,
            y: y,
            z: z
        });

        /*
         * If the declared number of nodes has
         * been reached, stop reading nodes.
         */

        if (
            expectedNodes > 0 &&
            points.length >= expectedNodes
        ) {
            break;
        }
    }

    return points;
}


/* ============================================================
   CHN DOWNLOAD
============================================================ */

document
.getElementById("chnDownloadBtn")
.addEventListener("click", function() {


    if (!chnOutputText) {

        alert(
            "Please process a CHN file first."
        );

        return;

    }


    const blob =
        new Blob(
            [chnOutputText],
            {
                type:
                    "text/plain;charset=utf-8"
            }
        );


    const url =
        URL.createObjectURL(blob);


    const link =
        document.createElement("a");


    link.href =
        url;


    const baseName =
        chnOriginalFileName
        .replace(
            /\.[^/.]+$/,
            ""
        );


    link.download =
        baseName +
        "_nodes.xyz";


    document.body.appendChild(link);

    link.click();

    document.body.removeChild(link);


    URL.revokeObjectURL(url);

});



/* ============================================================
   CHN CLEAR
============================================================ */

document
.getElementById("chnClearBtn")
.addEventListener("click", function() {


    document.getElementById(
        "chnFile"
    ).value = "";


    document.getElementById(
        "chnStatus"
    ).innerHTML = "";


    document.getElementById(
        "chnResult"
    ).textContent = "";


    document.getElementById(
        "chnDownloadBtn"
    ).style.display = "none";


    chnOutputText = "";

    chnOriginalFileName = "";

});



/* ============================================================
   CLEAR ALL
============================================================ */

document
.getElementById("clearAllBtn")
.addEventListener("click", function() {

    /* MTX */
    document.getElementById("mtxFile").value = "";
    document.getElementById("mtxZ").value = "0";
    document.getElementById("mtxStatus").innerHTML = "";
    document.getElementById("mtxResult").textContent = "";
    document.getElementById("mtxDownloadBtn").style.display = "none";
    mtxOutputText = "";
    mtxOriginalFileName = "";

    /* CHN */
    document.getElementById("chnFile").value = "";
    document.getElementById("chnStatus").innerHTML = "";
    document.getElementById("chnResult").textContent = "";
    document.getElementById("chnDownloadBtn").style.display = "none";
    chnOutputText = "";
    chnOriginalFileName = "";

    /* VDATUM */
    document.getElementById("vdatumFile").value = "";
    document.getElementById("surveyFile").value = "";
    document.getElementById("vdatumName").textContent = "No VDATUM file selected";
    document.getElementById("surveyName").textContent = "No survey file selected";
    document.getElementById("vdatumStatus").textContent = "Select both files to begin.";
    document.getElementById("vdatumDownloadSection").style.display = "none";
    document.getElementById("vdatumOutputFileName").textContent = "";
    document.getElementById("vdatumProgressContainer").style.display = "none";
    document.getElementById("vdatumProgressBar").value = 0;
    document.getElementById("vdatumProgressText").textContent = "0%";
    vdatumPoints = [];
    kdTree = null;
    outputBlob = null;
    outputFileName = "";

    /* Z adjustment */
    document.getElementById("zAdjustFile").value = "";
    document.getElementById("zAdjustment").value = "0";
    document.getElementById("invertZAdjust").checked = false;
    document.getElementById("zStatus").innerHTML = "";
    document.getElementById("zResult").textContent = "";
    document.getElementById("zDownloadBtn").style.display = "none";
    zOutputText = "";
    zOriginalFileName = "";

    window.scrollTo({
        top: 0,
        behavior: "smooth"
    });
});




/* ================= VDATUM TOOL ================= */



/* =====================================================
   GLOBAL VARIABLES
   ===================================================== */

let vdatumPoints = [];

let kdTree = null;

let outputBlob = null;

let outputFileName = "";



/* =====================================================
   VDATUM FILE NAME DISPLAY
   ===================================================== */

document
.getElementById("vdatumFile")
.addEventListener(
    "change",
    function () {

        if (this.files.length > 0) {

            document
            .getElementById("vdatumName")
            .textContent =
                this.files[0].name;

        }

        else {

            document
            .getElementById("vdatumName")
            .textContent =
                "No VDATUM file selected";

        }

    }
);



/* =====================================================
   SURVEY FILE NAME DISPLAY
   ===================================================== */

document
.getElementById("surveyFile")
.addEventListener(
    "change",
    function () {

        if (this.files.length > 0) {

            document
            .getElementById("surveyName")
            .textContent =
                this.files[0].name;

        }

        else {

            document
            .getElementById("surveyName")
            .textContent =
                "No survey file selected";

        }

    }
);



/* =====================================================
   PARSE XYZ FILE
   ===================================================== */

function parseXYZ(text) {

    const lines =
        text.split(/\r?\n/);


    const points = [];


    for (
        let i = 0;
        i < lines.length;
        i++
    ) {

        const line =
            lines[i].trim();


        if (!line) {

            continue;

        }


        const parts =
            line.split(/\s+/);


        if (
            parts.length < 3
        ) {

            continue;

        }


        const x =
            Number(parts[0]);


        const y =
            Number(parts[1]);


        const z =
            Number(parts[2]);


        if (

            Number.isFinite(x) &&

            Number.isFinite(y) &&

            Number.isFinite(z)

        ) {

            points.push({

                x: x,

                y: y,

                z: z

            });

        }

    }


    return points;

}



/* =====================================================
   KD TREE NODE
   ===================================================== */

class KDNode {

    constructor(point, axis) {

        this.point = point;

        this.axis = axis;

        this.left = null;

        this.right = null;

    }

}



/* =====================================================
   BUILD KD TREE
   ===================================================== */

function buildKDTree(
    points,
    depth = 0
) {

    if (
        points.length === 0
    ) {

        return null;

    }


    const axis =
        depth % 2;


    points.sort(
        function(a, b) {

            if (
                axis === 0
            ) {

                return a.x - b.x;

            }


            return a.y - b.y;

        }
    );


    const middle =
        Math.floor(
            points.length / 2
        );


    const node =
        new KDNode(
            points[middle],
            axis
        );


    node.left =
        buildKDTree(
            points.slice(
                0,
                middle
            ),
            depth + 1
        );


    node.right =
        buildKDTree(
            points.slice(
                middle + 1
            ),
            depth + 1
        );


    return node;

}



/* =====================================================
   XY DISTANCE SQUARED
   ===================================================== */

function distanceSquared(
    a,
    b
) {

    const dx =
        a.x - b.x;


    const dy =
        a.y - b.y;


    return (
        dx * dx +
        dy * dy
    );

}



/* =====================================================
   FIND CLOSEST VDATUM POINT
   ===================================================== */

function nearestPoint(
    node,
    target,
    best = null,
    bestDistance = Infinity
) {


    if (
        node === null
    ) {

        return {

            point: best,

            distance: bestDistance

        };

    }


    const currentDistance =
        distanceSquared(
            target,
            node.point
        );


    if (
        currentDistance <
        bestDistance
    ) {

        best =
            node.point;

        bestDistance =
            currentDistance;

    }


    const axis =
        node.axis;


    let difference;


    if (
        axis === 0
    ) {

        difference =
            target.x -
            node.point.x;

    }

    else {

        difference =
            target.y -
            node.point.y;

    }


    let nearBranch;

    let farBranch;


    if (
        difference < 0
    ) {

        nearBranch =
            node.left;

        farBranch =
            node.right;

    }

    else {

        nearBranch =
            node.right;

        farBranch =
            node.left;

    }


    let result =
        nearestPoint(

            nearBranch,

            target,

            best,

            bestDistance

        );


    best =
        result.point;


    bestDistance =
        result.distance;


    if (

        difference *
        difference <
        bestDistance

    ) {

        result =
            nearestPoint(

                farBranch,

                target,

                best,

                bestDistance

            );


        best =
            result.point;


        bestDistance =
            result.distance;

    }


    return {

        point: best,

        distance: bestDistance

    };

}



/* =====================================================
   STATUS FUNCTION
   ===================================================== */

function setStatus(
    message
) {

    document
    .getElementById("vdatumStatus")
    .textContent =
        message;

}



/* =====================================================
   PROCESS BUTTON
   ===================================================== */

document
.getElementById("vdatumProcessButton")
.addEventListener(
    "click",
    async function () {

        const vdatumRoundOn =
            document.getElementById("vdatumRound").checked;


        /* ---------------------------------------------
           GET FILES
           --------------------------------------------- */

        const vdatumFile =
            document
            .getElementById(
                "vdatumFile"
            )
            .files[0];


        const surveyFile =
            document
            .getElementById(
                "surveyFile"
            )
            .files[0];



        /* ---------------------------------------------
           CHECK FILES
           --------------------------------------------- */

        if (!vdatumFile) {

            alert(
                "Please select the VDATUM XYZ file."
            );

            return;

        }


        if (!surveyFile) {

            alert(
                "Please select the survey / second XYZ file."
            );

            return;

        }



        /* ---------------------------------------------
           PROCESS BUTTON
           --------------------------------------------- */

        const processButton =
            document
            .getElementById(
                "vdatumProcessButton"
            );


        processButton.disabled =
            true;


        processButton.textContent =
            "Processing...";



        /* ---------------------------------------------
           PROGRESS
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumProgressContainer"
        )
        .style.display =
            "block";


        document
        .getElementById(
            "vdatumProgressBar"
        )
        .value =
            0;


        document
        .getElementById(
            "vdatumProgressText"
        )
        .textContent =
            "0%";



        /* ---------------------------------------------
           HIDE OLD DOWNLOAD
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumDownloadSection"
        )
        .style.display =
            "none";


        outputBlob =
            null;


        outputFileName =
            "";



        try {


            /* =========================================
               READ VDATUM FILE
               ========================================= */

            setStatus(
                "Reading VDATUM file..."
            );


            const vdatumText =
                await vdatumFile.text();


            vdatumPoints =
                parseXYZ(
                    vdatumText
                );


            if (
                vdatumPoints.length === 0
            ) {

                throw new Error(
                    "No valid XYZ points were found in the VDATUM file."
                );

            }


            setStatus(

                "VDATUM file loaded.\n\n" +

                "VDATUM points: " +

                vdatumPoints
                .length
                .toLocaleString() +

                "\n\nBuilding closest-point search tree..."

            );


            await new Promise(
                function(resolve) {

                    setTimeout(
                        resolve,
                        50
                    );

                }
            );



            /* =========================================
               BUILD KD TREE
               ========================================= */

            kdTree =
                buildKDTree(
                    vdatumPoints
                );



            /* =========================================
               READ SURVEY FILE
               ========================================= */

            setStatus(
                "Reading survey XYZ file..."
            );


            const surveyText =
                await surveyFile.text();


            const surveyLines =
                surveyText.split(
                    /\r?\n/
                );


            const outputLines =
                [];


            let validPoints =
                0;


            let unchangedLines =
                0;



            /* =========================================
               PROCESS SURVEY POINTS
               ========================================= */

            for (
                let i = 0;
                i < surveyLines.length;
                i++
            ) {


                const originalLine =
                    surveyLines[i];


                const line =
                    originalLine.trim();



                /* -------------------------------------
                   BLANK LINE
                   ------------------------------------- */

                if (!line) {

                    outputLines.push(
                        originalLine
                    );

                    unchangedLines++;

                    continue;

                }



                /* -------------------------------------
                   SPLIT XYZ
                   ------------------------------------- */

                const parts =
                    line.split(
                        /\s+/
                    );


                if (
                    parts.length < 3
                ) {

                    outputLines.push(
                        originalLine
                    );

                    unchangedLines++;

                    continue;

                }



                /* -------------------------------------
                   READ XYZ
                   ------------------------------------- */

                const x =
                    Number(
                        parts[0]
                    );


                const y =
                    Number(
                        parts[1]
                    );


                const z =
                    Number(
                        parts[2]
                    );



                /* -------------------------------------
                   INVALID LINE
                   ------------------------------------- */

                if (

                    !Number.isFinite(x) ||

                    !Number.isFinite(y) ||

                    !Number.isFinite(z)

                ) {

                    outputLines.push(
                        originalLine
                    );

                    unchangedLines++;

                    continue;

                }



                /* -------------------------------------
                   FIND CLOSEST VDATUM POINT
                   ------------------------------------- */

                const nearest =
                    nearestPoint(

                        kdTree,

                        {
                            x: x,
                            y: y
                        }

                    );


                const vdatumPoint =
                    nearest.point;



                /* -------------------------------------
                   CALCULATE NEW Z
                   ------------------------------------- */

                const newZ =
                    z +
                    vdatumPoint.z;



                /* -------------------------------------
                   OUTPUT FORMAT

                   X = 2 decimals
                   Y = 2 decimals
                   Z = 2 decimals
                   ------------------------------------- */

                const outputLine =

                    x.toFixed(2) +
                    " " +

                    y.toFixed(2) +
                    " " +

                    roundHalfUp(newZ, vdatumRoundOn ? 1 : 2);



                outputLines.push(
                    outputLine
                );


                validPoints++;



                /* -------------------------------------
                   UPDATE PROGRESS
                   ------------------------------------- */

                if (
                    i % 5000 === 0
                ) {


                    const percent =

                        (
                            i /
                            surveyLines.length
                        ) * 100;


                    document
                    .getElementById(
                        "vdatumProgressBar"
                    )
                    .value =
                        percent;


                    document
                    .getElementById(
                        "vdatumProgressText"
                    )
                    .textContent =

                        Math.round(
                            percent
                        ) +
                        "%";


                    setStatus(

                        "Processing survey points...\n\n" +

                        "Points processed: " +

                        validPoints
                        .toLocaleString() +

                        "\n\nProgress: " +

                        Math.round(
                            percent
                        ) +

                        "%"

                    );


                    await new Promise(
                        function(resolve) {

                            setTimeout(
                                resolve,
                                0
                            );

                        }
                    );

                }

            }



            /* =========================================
               COMPLETE
               ========================================= */

            document
            .getElementById(
                "vdatumProgressBar"
            )
            .value =
                100;


            document
            .getElementById(
                "vdatumProgressText"
            )
            .textContent =
                "100%";



            /* =========================================
               CREATE OUTPUT TEXT
               ========================================= */

            const outputText =
                outputLines.join(
                    "\n"
                );



            /* =========================================
               CREATE OUTPUT BLOB
               ========================================= */

            outputBlob =
                new Blob(

                    [outputText],

                    {
                        type:
                            "text/plain;charset=utf-8"
                    }

                );



            /* =========================================
               CREATE OUTPUT FILE NAME
               ========================================= */

            const originalName =
                surveyFile.name;


            const baseName =
                originalName.replace(
                    /\.(xyz|txt)$/i,
                    ""
                );


            outputFileName =
                baseName +
                "_VDATUM_ADJUSTED.xyz";



            /* =========================================
               SHOW DOWNLOAD SECTION
               
               IMPORTANT:
               NO AUTOMATIC DOWNLOAD
               ========================================= */

            document
            .getElementById(
                "vdatumDownloadSection"
            )
            .style.display =
                "block";


            document
            .getElementById(
                "vdatumOutputFileName"
            )
            .textContent =
                outputFileName;



            /* =========================================
               FINAL STATUS
               ========================================= */

            setStatus(

                "PROCESSING COMPLETE\n\n" +

                "VDATUM points: " +

                vdatumPoints
                .length
                .toLocaleString() +

                "\n\n" +

                "Survey points processed: " +

                validPoints
                .toLocaleString() +

                "\n\n" +

                "Unchanged/non-XYZ lines: " +

                unchangedLines
                .toLocaleString() +

                "\n\n" +

                "Calculation:\n" +

                "New Z = Survey Z + VDATUM Z" +

                "\n\n" +

                "Output file is ready.\n" +

                "Click the green Download XYZ File button."

            );


        }


        catch (error) {


            console.error(
                error
            );


            setStatus(

                "ERROR\n\n" +
                error.message

            );


            alert(

                "An error occurred:\n\n" +
                error.message

            );

        }


        finally {


            processButton.disabled =
                false;


            processButton.textContent =
                "Process XYZ File";

        }

    }
);



/* =====================================================
   DOWNLOAD BUTTON

   THIS IS THE ONLY DOWNLOAD ACTION.
   ===================================================== */

document
.getElementById(
    "vdatumDownloadButton"
)
.addEventListener(
    "click",
    function () {


        if (!outputBlob) {

            alert(
                "Please process the XYZ file first."
            );

            return;

        }


        const url =
            URL.createObjectURL(
                outputBlob
            );


        const link =
            document.createElement(
                "a"
            );


        link.href =
            url;


        link.download =
            outputFileName;


        document
        .body
        .appendChild(
            link
        );


        link.click();


        document
        .body
        .removeChild(
            link
        );


        setTimeout(
            function () {

                URL.revokeObjectURL(
                    url
                );

            },
            1000
        );

    }
);



/* =====================================================
   REFRESH / CLEAR ALL BUTTON
   ===================================================== */

document
.getElementById(
    "vdatumRefreshButton"
)
.addEventListener(
    "click",
    function () {


        /* ---------------------------------------------
           CLEAR FILE INPUTS
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumFile"
        )
        .value =
            "";


        document
        .getElementById(
            "surveyFile"
        )
        .value =
            "";



        /* ---------------------------------------------
           CLEAR FILE NAMES
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumName"
        )
        .textContent =
            "No VDATUM file selected";


        document
        .getElementById(
            "surveyName"
        )
        .textContent =
            "No survey file selected";



        /* ---------------------------------------------
           CLEAR DATA
           --------------------------------------------- */

        vdatumPoints =
            [];


        kdTree =
            null;


        outputBlob =
            null;


        outputFileName =
            "";



        /* ---------------------------------------------
           HIDE DOWNLOAD
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumDownloadSection"
        )
        .style.display =
            "none";


        document
        .getElementById(
            "vdatumOutputFileName"
        )
        .textContent =
            "";



        /* ---------------------------------------------
           RESET PROGRESS
           --------------------------------------------- */

        document
        .getElementById(
            "vdatumProgressContainer"
        )
        .style.display =
            "none";


        document
        .getElementById(
            "vdatumProgressBar"
        )
        .value =
            0;


        document
        .getElementById(
            "vdatumProgressText"
        )
        .textContent =
            "0%";



        /* ---------------------------------------------
           RESET PROCESS BUTTON
           --------------------------------------------- */

        const processButton =
            document
            .getElementById(
                "vdatumProcessButton"
            );


        processButton.disabled =
            false;


        processButton.textContent =
            "Process XYZ File";



        /* ---------------------------------------------
           RESET STATUS
           --------------------------------------------- */

        setStatus(
            "Select both files to begin."
        );



        /* ---------------------------------------------
           SCROLL TO TOP
           --------------------------------------------- */

        window.scrollTo(
            {
                top: 0,
                behavior: "smooth"
            }
        );

    }
);




/* ================= Z ADJUST TOOL ================= */


let zOutputText = "";
let zOriginalFileName = "";


document.getElementById("zProcessBtn").addEventListener("click", function () {

    const zRoundOn = document.getElementById("zRound").checked;

    const zAdjustFile =
        document.getElementById("zAdjustFile");

    const adjustmentInput =
        document.getElementById("zAdjustment");

    const invertZInput =
        document.getElementById("invertZAdjust");

    const zStatus =
        document.getElementById("zStatus");

    const zResult =
        document.getElementById("zResult");

    const zDownloadBtn =
        document.getElementById("zDownloadBtn");


    if (!zAdjustFile.files.length) {

        alert("Please select an XYZ or TXT file.");

        return;
    }


    const zAdjustment =
        Number(adjustmentInput.value);


    if (!Number.isFinite(zAdjustment)) {

        alert("Please enter a valid zAdjustment value.");

        return;
    }


    const invertZAdjust =
        invertZInput.checked;


    const file =
        zAdjustFile.files[0];


    zOriginalFileName =
        file.name;


    const reader =
        new FileReader();


    reader.onload = function (event) {

        const text =
            event.target.zResult;


        const lines =
            text.split(/\r?\n/);


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

            const parts =
                line.trim().split(/\s+/);


            if (parts.length >= 3) {

                const x =
                    Number(parts[0]);

                const y =
                    Number(parts[1]);

                const z =
                    Number(parts[2]);


                if (
                    Number.isFinite(x) &&
                    Number.isFinite(y) &&
                    Number.isFinite(z)
                ) {


                    /*
                     * Apply Z zAdjustment
                     */

                    let newZ =
                        z + zAdjustment;


                    /*
                     * Invert Z if selected
                     */

                    if (invertZAdjust) {

                        newZ =
                            -newZ;
                    }


                    /*
                     * Format output:
                     *
                     * X = 2 decimals
                     * Y = 2 decimals
                     * Z = 1 decimal
                     */

                    processedLines.push(

                        x.toFixed(zRoundOn ? 2 : 3) + " " +
                        y.toFixed(zRoundOn ? 2 : 3) + " " +
                        roundHalfUp(newZ, zRoundOn ? 1 : 3)

                    );


                    validPoints++;


                } else {

                    processedLines.push(line);

                    unchangedLines++;
                }


            } else {

                /*
                 * Keep lines that don't contain
                 * at least X Y Z unchanged.
                 */

                processedLines.push(line);

                unchangedLines++;
            }

        }


        /*
         * Create final output
         */

        zOutputText =
            processedLines.join("\n");


        /*
         * Display processing information
         */

        zStatus.innerHTML =

            "<div class='info'>" +

            "<strong>Processing complete.</strong><br>" +

            "Points processed: " +
            validPoints.toLocaleString() +
            "<br>" +

            "Lines unchanged: " +
            unchangedLines.toLocaleString() +
            "<br>" +

            "Z zAdjustment: " +
            zAdjustment.toFixed(2) +
            "<br>" +

            "Invert Z: " +
            (invertZAdjust ? "YES" : "NO") +
            "<br>" +

            (zRoundOn ? "Output: X Y 2 decimals, Z 1 decimal" : "Output: X Y Z 3 decimals") +

            "</div>";


        /*
         * Show first 10 processed lines
         */

        zResult.textContent =
            processedLines
                .slice(0, 10)
                .join("\n");


        /*
         * Show download button
         */

        zDownloadBtn.style.display =
            "inline-block";

    };


    reader.readAsText(file);

});


/*
 * Download corrected file
 */

document.getElementById("zDownloadBtn").addEventListener("click", function () {

    if (!zOutputText) {

        alert("Please process a file first.");

        return;
    }


    /*
     * Create downloadable text file
     */

    const blob =
        new Blob(
            [zOutputText],
            {
                type:
                    "text/plain;charset=utf-8"
            }
        );


    const url =
        URL.createObjectURL(blob);


    const link =
        document.createElement("a");


    link.href =
        url;


    /*
     * Create output filename
     */

    const baseName =
        zOriginalFileName
            .replace(/\.[^/.]+$/, "");


    link.download =
        baseName + "_Z_ADJUSTED.txt";


    document.body.appendChild(link);


    link.click();


    document.body.removeChild(link);


    URL.revokeObjectURL(url);

});



/* ============================================================
   GLOBAL CLEAR ALL
============================================================ */

document
.getElementById("clearAllBtn")
.addEventListener("click", function() {

    /* MTX */
    if (document.getElementById("mtxFile"))
        document.getElementById("mtxFile").value = "";

    if (document.getElementById("mtxZ"))
        document.getElementById("mtxZ").value = "0";

    if (document.getElementById("mtxStatus"))
        document.getElementById("mtxStatus").innerHTML = "";

    if (document.getElementById("mtxResult"))
        document.getElementById("mtxResult").textContent = "";

    if (document.getElementById("mtxDownloadBtn"))
        document.getElementById("mtxDownloadBtn").style.display = "none";

    if (typeof mtxOutputText !== "undefined") mtxOutputText = "";
    if (typeof mtxOriginalFileName !== "undefined") mtxOriginalFileName = "";

    /* CHN */
    if (document.getElementById("chnFile"))
        document.getElementById("chnFile").value = "";

    if (document.getElementById("chnStatus"))
        document.getElementById("chnStatus").innerHTML = "";

    if (document.getElementById("chnResult"))
        document.getElementById("chnResult").textContent = "";

    if (document.getElementById("chnDownloadBtn"))
        document.getElementById("chnDownloadBtn").style.display = "none";

    if (typeof chnOutputText !== "undefined") chnOutputText = "";
    if (typeof chnOriginalFileName !== "undefined") chnOriginalFileName = "";

    /* VDATUM */
    if (document.getElementById("vdatumFile"))
        document.getElementById("vdatumFile").value = "";

    if (document.getElementById("surveyFile"))
        document.getElementById("surveyFile").value = "";

    if (document.getElementById("vdatumName"))
        document.getElementById("vdatumName").textContent =
            "No VDATUM file selected";

    if (document.getElementById("surveyName"))
        document.getElementById("surveyName").textContent =
            "No survey file selected";

    if (typeof vdatumPoints !== "undefined") vdatumPoints = [];
    if (typeof kdTree !== "undefined") kdTree = null;
    if (typeof vdatumOutputBlob !== "undefined") vdatumOutputBlob = null;
    if (typeof vdatumOutputFileName !== "undefined") vdatumOutputFileName = "";

    if (document.getElementById("vdatumDownloadSection"))
        document.getElementById("vdatumDownloadSection").style.display = "none";

    if (document.getElementById("vdatumOutputFileName"))
        document.getElementById("vdatumOutputFileName").textContent = "";

    if (document.getElementById("vdatumProgressContainer"))
        document.getElementById("vdatumProgressContainer").style.display = "none";

    if (document.getElementById("vdatumProgressBar"))
        document.getElementById("vdatumProgressBar").value = 0;

    if (document.getElementById("vdatumProgressText"))
        document.getElementById("vdatumProgressText").textContent = "0%";

    if (document.getElementById("vdatumStatus"))
        document.getElementById("vdatumStatus").textContent =
            "Select both files to begin.";

    /* Z ADJUST / INVERT */
    if (document.getElementById("zAdjustFile"))
        document.getElementById("zAdjustFile").value = "";

    if (document.getElementById("zAdjustment"))
        document.getElementById("zAdjustment").value = "0";

    if (document.getElementById("invertZAdjust"))
        document.getElementById("invertZAdjust").checked = false;

    if (document.getElementById("zStatus"))
        document.getElementById("zStatus").innerHTML = "";

    if (document.getElementById("zResult"))
        document.getElementById("zResult").textContent = "";

    if (document.getElementById("zDownloadBtn"))
        document.getElementById("zDownloadBtn").style.display = "none";

    if (typeof zOutputText !== "undefined") zOutputText = "";
    if (typeof zOriginalFileName !== "undefined") zOriginalFileName = "";
});

</script>


<script>

/* ============================================================
   COORDINATE CONVERTER TAB (NJ 2900 / NY East 3101 / NY Long Island 3104)
   Wrapped in its own scope so it cannot clash with the other tools.
============================================================ */

(function () {

/* ---------- Projection math (GRS80, US survey foot) ---------- */
const A_ = 6378137.0, F_ = 1 / 298.257222101, E2 = 2 * F_ - F_ * F_, E = Math.sqrt(E2);
const FT = 1200 / 3937; // metres per US survey foot
const rad = d => d * Math.PI / 180;
const {sin, cos, tan, atan, atan2, asin, sinh, cosh, tanh, log, sqrt, PI} = Math;
const atanh = Math.atanh;

/* Transverse Mercator (used by NJ 2900 and NY East 3101) */
function makeTM(p) {
  const n = F_ / (2 - F_);
  const AK = A_ / (1 + n) * (1 + n ** 2 / 4 + n ** 4 / 64);
  const AL = [n / 2 - 2 * n ** 2 / 3 + 5 * n ** 3 / 16, 13 * n ** 2 / 48 - 3 * n ** 3 / 5, 61 * n ** 3 / 240];
  const BE = [n / 2 - 2 * n ** 2 / 3 + 37 * n ** 3 / 96, n ** 2 / 48 + n ** 3 / 15, 17 * n ** 3 / 480];
  const conf = lat => atan(sinh(atanh(sin(lat)) - E * atanh(E * sin(lat))));
  const arc = lat => { const x = conf(lat); return AK * (x + AL.reduce((s, a, j) => s + a * sin(2 * (j + 1) * x), 0)); };
  const M0 = p.k0 * arc(p.lat0);
  return {
    toLL(Em, Nm) {
      const xi = (Nm - p.fn + M0) / (p.k0 * AK), eta = (Em - p.fe) / (p.k0 * AK);
      let xi_ = xi, eta_ = eta;
      for (let j = 0; j < 3; j++) {
        xi_ -= BE[j] * sin(2 * (j + 1) * xi) * cosh(2 * (j + 1) * eta);
        eta_ -= BE[j] * cos(2 * (j + 1) * xi) * sinh(2 * (j + 1) * eta);
      }
      const chi = asin(sin(xi_) / cosh(eta_));
      let lat = chi;
      for (let i = 0; i < 10; i++) lat = asin(tanh(atanh(sin(chi)) + E * atanh(E * sin(lat))));
      return [lat, p.lon0 + atan2(sinh(eta_), cos(xi_))];
    },
    fromLL(lat, lon) {
      const c = conf(lat), dl = lon - p.lon0;
      const xi_ = atan2(tan(c), cos(dl)), eta_ = atanh(sin(dl) * cos(c));
      let xi = xi_, eta = eta_;
      for (let j = 0; j < 3; j++) {
        xi += AL[j] * sin(2 * (j + 1) * xi_) * cosh(2 * (j + 1) * eta_);
        eta += AL[j] * cos(2 * (j + 1) * xi_) * sinh(2 * (j + 1) * eta_);
      }
      return [p.fe + p.k0 * AK * eta, p.fn + p.k0 * AK * xi - M0];
    }
  };
}

/* Lambert Conformal Conic, 2 standard parallels (NY Long Island 3104) */
function makeLCC(p) {
  const mm = q => cos(q) / sqrt(1 - E2 * sin(q) ** 2);
  const tt = q => tan(PI / 4 - q / 2) / (((1 - E * sin(q)) / (1 + E * sin(q))) ** (E / 2));
  const n = (log(mm(p.p1)) - log(mm(p.p2))) / (log(tt(p.p1)) - log(tt(p.p2)));
  const F = mm(p.p1) / (n * tt(p.p1) ** n), R0 = A_ * F * tt(p.p0) ** n;
  return {
    fromLL(lat, lon) {
      const r = A_ * F * tt(lat) ** n, th = n * (lon - p.lon0);
      return [p.fe + r * sin(th), R0 - r * cos(th)];
    },
    toLL(Em, Nm) {
      const x = Em - p.fe, y = R0 - Nm;
      const r = sqrt(x * x + y * y), th = atan2(x, y);
      const t = (r / (A_ * F)) ** (1 / n);
      let lat = PI / 2 - 2 * atan(t);
      for (let i = 0; i < 10; i++) lat = PI / 2 - 2 * atan(t * ((1 - E * sin(lat)) / (1 + E * sin(lat))) ** (E / 2));
      return [lat, th / n + p.lon0];
    }
  };
}

const ZONES = {
  NJ:   {label: "NJ FIPS 2900 (EPSG:3424)",              tag: "NJ_FIPS2900",
         ...makeTM({lat0: rad(38 + 50 / 60), lon0: rad(-74.5), k0: 0.9999, fe: 150000, fn: 0})},
  NYE:  {label: "NY East FIPS 3101 (EPSG:2260)",         tag: "NYE_FIPS3101",
         ...makeTM({lat0: rad(38 + 50 / 60), lon0: rad(-74.5), k0: 0.9999, fe: 150000, fn: 0})},
  NYLI: {label: "NY Long Island FIPS 3104 (EPSG:2263)",  tag: "NYLI_FIPS3104",
         ...makeLCC({p1: rad(41 + 2 / 60), p2: rad(40 + 40 / 60), p0: rad(40 + 10 / 60), lon0: rad(-74), fe: 300000})}
};

/* coordinates in US survey feet in and out */
function convertXY(from, to, x, y) {
  const [la, lo] = ZONES[from].toLL(x * FT, y * FT);
  const [e, n] = ZONES[to].fromLL(la, lo);
  return [e / FT, n / FT];
}


function cvRoundHalfUp(v, d) {
  const f = Math.pow(10, d);
  return (Math.sign(v) * Math.round(Math.abs(v) * f + 1e-9) / f).toFixed(d);
}
const isNum = t => /^[+-]?(\d+\.?\d*|\.\d+)$/.test(t || "");
/* returns index of the X column (0 = X Y [Z], 1 = ID X Y [Z]) or -1 if the line is not coordinates */
function detectIdx(p) {
  if (isNum(p[0]) && isNum(p[1])) {
    return (p.length >= 4 && /^\d+$/.test(p[0]) && isNum(p[2]) && isNum(p[3])) ? 1 : 0;
  }
  return (isNum(p[1]) && isNum(p[2])) ? 1 : -1;
}

function cvConvertText(text, dir, round) {
  const [from, to] = dir.split(">");
  const lines = text.split(/\r?\n/);
  const first = lines.find(l => l.trim()) || "";
  const sep = first.includes("\t") ? "\t" : first.includes(",") ? "," : " ";
  const split = line => sep === " " ? line.trim().split(/\s+/) : line.split(sep).map(s => s.trim());
  let idx = -1;
  for (const l of lines) { if (!l.trim()) continue; const d = detectIdx(split(l)); if (d !== -1) { idx = d; break; } }
  let ok = 0; const bad = []; const rows = []; const out = [];
  lines.forEach((line, i) => {
    if (!line.trim()) { out.push(line); return; }
    const parts = split(line);
    const x = parseFloat(parts[idx]), y = parseFloat(parts[idx + 1]);
    if (idx < 0 || !isFinite(x) || !isFinite(y)) { bad.push(i + 1); out.push(line); return; }
    const [nx, ny] = convertXY(from, to, x, y);
    let z = parts[idx + 2];
    if (round && z !== undefined && isNum(z)) z = cvRoundHalfUp(parseFloat(z), 1);
    if (rows.length < 10) rows.push({id: idx ? parts[0] : "", x, y, z: z === undefined ? "" : z, nx, ny});
    parts[idx] = nx.toFixed(2); parts[idx + 1] = ny.toFixed(2);
    if (z !== undefined) parts[idx + 2] = z;
    ok++;
    out.push(parts.join(sep === " " ? " " : sep));
  });
  return {text: out.join("\n"), ok, bad, rows, hasId: idx === 1};
}

if (typeof document !== "undefined") {
  const $ = id => document.getElementById(id);
  const esc = t => String(t).replace(/[&<>]/g, c => ({"&": "&amp;", "<": "&lt;", ">": "&gt;"}[c]));
  let src = "", srcName = "", result = "";

  function resetOutput() {
    result = "";
    $("cvDownloadBtn").style.display = "none";
    $("cvPreview").innerHTML = "";
    $("cvStatus").innerHTML = "";
  }
  function note() {
    const d = $("cvDir").value;
    $("cvNote").style.display = (d === "NJ>NYE" || d === "NYE>NJ") ? "block" : "none";
  }

  $("cvFile").addEventListener("change", e => {
    const f = e.target.files[0];
    if (!f) { $("cvConvertBtn").disabled = true; return; }
    const r = new FileReader();
    r.onload = () => {
      src = String(r.result); srcName = f.name; resetOutput();
      $("cvConvertBtn").disabled = false;
    };
    r.onerror = () => { $("cvStatus").innerHTML = '<div class="error">Could not read the file.</div>'; };
    r.readAsText(f);
  });
  $("cvDir").addEventListener("change", () => { resetOutput(); note(); });
  $("cvRound").addEventListener("change", resetOutput);
  note();

  $("cvConvertBtn").addEventListener("click", () => {
    const dir = $("cvDir").value;
    const [from, to] = dir.split(">");
    const res = cvConvertText(src, dir, $("cvRound").checked);
    if (!res.ok) {
      resetOutput();
      $("cvStatus").innerHTML = '<div class="error">No valid coordinate rows found.</div>';
      return;
    }
    result = res.text.replace(/\n*$/, "\n");
    const skipped = res.bad.length
      ? " " + res.bad.length + " line(s) skipped (" + res.bad.slice(0, 10).join(", ") + (res.bad.length > 10 ? ", ..." : "") + ")."
      : "";
    $("cvStatus").innerHTML = '<div class="success">Converted ' + res.ok + ' point' + (res.ok === 1 ? '' : 's') +
      ' to ' + ZONES[to].label + '.' + (res.hasId ? ' ID column detected.' : '') + skipped + '</div>';
    $("cvDownloadBtn").style.display = "inline-block";
    let h = "<h3>First " + res.rows.length + " converted points</h3><table><tr>" +
      (res.hasId ? "<th>ID</th>" : "") + "<th>Input X</th><th>Input Y</th><th>Z</th><th>Output X</th><th>Output Y</th></tr>";
    res.rows.forEach(r => {
      h += "<tr>" + (res.hasId ? "<td>" + esc(r.id) + "</td>" : "") + "<td>" + r.x.toFixed(2) + "</td><td>" + r.y.toFixed(2) +
        "</td><td>" + esc(r.z) + "</td><td>" + r.nx.toFixed(2) + "</td><td>" + r.ny.toFixed(2) + "</td></tr>";
    });
    $("cvPreview").innerHTML = h + "</table>";
  });

  $("cvDownloadBtn").addEventListener("click", () => {
    if (!result) return;
    const tag = ZONES[$("cvDir").value.split(">")[1]].tag;
    const name = srcName.replace(/\.[^/.]+$/, "") + "_" + tag + ".xyz";
    const url = URL.createObjectURL(new Blob([result], {type: "text/plain"}));
    const a = document.createElement("a");
    a.href = url; a.download = name;
    document.body.appendChild(a); a.click(); document.body.removeChild(a);
    setTimeout(() => URL.revokeObjectURL(url), 1000);
  });

  /* Clear All button */
  const clr = $("clearAllBtn");
  if (clr) clr.addEventListener("click", () => {
    $("cvFile").value = ""; src = ""; srcName = "";
    $("cvConvertBtn").disabled = true;
    $("cvDir").selectedIndex = 0; $("cvRound").checked = false;
    resetOutput(); note();
  });
}

window.__cvTest = {convertXY, cvConvertText};
})();

</script>
</body>
</html>
