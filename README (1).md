# EEG Web Annotator

**A browser-based tool for labeling EEG artifacts and seizures using TUH standard codes. Open an EDF file, annotate it, and export a CSV. Nothing to install.**

**Try it now:** https://YOUR-USERNAME.github.io/eeg-web-annotator/ (tap **Demo**)

**Abdulmalik Lawal**: EEG technician with 400+ diagnostic recordings in pediatric neurology, now building tools for EEG annotation and artifact review.

## What it does
- Opens standard `.edf` / EDF+ recordings directly in your browser
- Lets you drag to select a segment and label it with one tap or key press
- Shows every label on an overview strip so you can jump anywhere in the recording
- Reads events already stored in the file and imports or exports annotations as CSV
- Works on phones and tablets as well as computers

The **Demo** button opens a synthetic 2-minute recording with example labels already placed (eye movement, muscle, electrode artifacts and a seizure), so you can see a finished annotation in one tap.

## Label codes
The codes follow the conventions of the Temple University Hospital (TUH) EEG corpora, so annotations line up with published datasets.

| Key | Code | Meaning |
|---|---|---|
| 1 | eyem | Eye movement (blinks, lateral eye movements) |
| 2 | musc | Muscle artifact |
| 3 | elec | Electrode pop, electrostatic and lead artifacts |
| 4 | chew | Chewing artifact |
| 5 | shiv | Shivering artifact |
| 6 | bckg | Background (no event of interest) |
| 7 | seiz | Seizure |

## Try it with real data
1. Download a public EDF file, for example `chb05_06.edf` from the [CHB-MIT Scalp EEG Database](https://www.physionet.org/content/chbmit/1.0.0/chb05/).
2. Tap **Load EEG** and choose the file.
3. Tap **Import labels** and choose `labels/chb05_06_seizure_labels.csv`. The view jumps to the seizure at 417-532 seconds.

Only the first 10 minutes of a file load, and BDF files are not supported.

## Privacy
Everything runs in your browser and no data is uploaded. The demo data is synthetic. Real examples use public datasets only; no patient recordings are included.

## Why I built this
I recorded over 400 diagnostic EEG studies as a technician in a pediatric neurology hospital. I built this tool to make labeling artifacts and seizures quick and consistent, using the same codes as public clinical datasets.

## Contact
Available for remote EEG annotation and review work. Message me on LinkedIn: [YOUR LINKEDIN LINK]

## License
MIT
