# EEG Web Annotator

A browser-based tool for labeling EEG events and artifacts. It opens EDF recordings directly in the browser, so there is nothing to install and no code to run. It is one static HTML file you can host on GitHub Pages.

**Abdulmalik Lawal**: EEG technician with 400+ diagnostic recordings in pediatric neurology, now building tools for EEG annotation and artifact review.

## Features
- Opens `.edf` / EDF+ files directly
- Shows events already stored in the file 
- Multichannel viewer with paging, channel paging, window length, gain and an optional 1-40 Hz display filter
- Drag to select a segment, tap a label or press keys 1-7 to apply it
- Overview strip under the traces shows where every label sits in the recording; tap it, or type a time in **Go to s**, to jump there
- Works on touch screens
- Import and export annotations as CSV (`onset,duration,description`), a format many EEG programs can read
- Built-in demo: a synthetic 2-minute recording with example labels already placed (eye movement, muscle, electrode artifacts and a seizure).

## Quick start
1. Open `index.html` in a browser and click **Demo**. The strip under the traces shows the labels; tap it to jump around.
2. Drag across the traces, then press `1` to label a blink or a different artifact.


Notes:
- Only the first 10 minutes of a file are loaded, to keep the page fast.
- Recordings above 256 Hz are thinned for display. Event times are unaffected.
- The 1-40 Hz view is for display only; the file is not changed.


## Labels
The label codes follow the conventions of the Temple University Hospital (TUH) EEG corpora from the Neural Engineering Data Consortium. 

| Key | Code | Meaning |
|---|---|---|
| 1 | eyem | Eye movement (blinks, lateral eye movements) |
| 2 | musc | Muscle artifact |
| 3 | elec | Electrode pop, electrostatic and lead artifacts |
| 4 | chew | Chewing artifact |
| 5 | shiv | Shivering artifact |
| 6 | bckg | Background (no event of interest) |
| 7 | seiz | Seizure |






## Roadmap
- [ ] Per-channel labels
- [ ] Autosave to browser storage
- [ ] Inter-rater agreement (Cohen's kappa)
- [ ] BDF (24-bit) support

## License
MIT, TUH
