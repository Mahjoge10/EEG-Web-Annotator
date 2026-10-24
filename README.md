# EEG Web Annotator

A browser-based tool for labeling EEG events and artifacts. It opens EDF recordings directly in the browser, so there is nothing to install and no code to run. It is one static HTML file you can host on GitHub Pages.

**Abdulmalik Lawal**: EEG technician with 400+ diagnostic recordings in pediatric neurology, now building tools for EEG annotation and artifact review.

## Features
- Opens `.edf` / EDF+ files directly
- Shows events already stored in the file (for example PhysioNet T1/T2 markers)
- Multichannel viewer with paging, channel paging, window length, gain and an optional 1-40 Hz display filter
- Drag to select a segment, tap a label or press keys 1-6 to apply it
- Works on touch screens
- Import and export annotations as CSV (`onset,duration,description`), a format many EEG programs can read
- Built-in synthetic demo

## Quick start
1. Open `index.html` in a browser and click **Demo**.
2. Drag across the traces, then press `1` to label a blink.
3. Click **Export CSV**.

## Use real recordings (public datasets only)
1. Download an EDF file, for example a run from the PhysioNet EEG Motor Movement/Imagery dataset, CHB-MIT, or Sleep-EDF.
2. Click **Load EEG (.edf / .json)** and choose the file.
3. Use **Ch up / Ch down** and the channel count menu to move through channels.
4. Annotate and export your CSV.

Notes:
- Only the first 10 minutes of a file are loaded, to keep the page fast.
- Recordings above 256 Hz are thinned for display. Event times are unaffected.
- The 1-40 Hz view is for display only; the file is not changed.
- Events stored in the EDF are shown with your labels and included in the exported CSV. Delete any you do not want from the list.

## Labels
| Key | Label |
|---|---|
| 1 | BAD_blink |
| 2 | BAD_muscle |
| 3 | BAD_electrode_pop |
| 4 | BAD_movement |
| 5 | BAD_line_noise |
| 6 | EVENT_custom |




## License
MIT
