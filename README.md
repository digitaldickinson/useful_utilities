# useful_utilities

Odds and ends for managing day-to-day uni work. Most are single HTML files: download one, open it in a browser, and it runs locally with no uploads (some load libraries from a CDN).

## Files

| File | What it does |
| --- | --- |
| `mailmerge_to_customFilenameDoc.html` | Mail merge from a Word template and a spreadsheet into individually named Word docs, replacing `{{tags}}`. Handy for generating named feedback sheets. |
| `moodles.html` | Takes a Moodle submissions zip (plus an optional grading CSV) and generates personalised feedback docs named to work with Moodle's bulk feedback upload. Tuned to my uni's Moodle; naming may differ elsewhere. |
| `moodle-feedback-helper-v3.zip` | Edge/Chrome extension that matches files in a local feedback folder to the student you're grading in Moodle, so you can drag or upload them without hunting. See below. |
| `Turnitin_rubric_viewer.html` | Opens a Turnitin rubric (`.rbc`), lets you edit and add criteria, then save it back as `.rbc` or export it as a landscape Word doc. |
| `powerpuller.html` | Pulls text, speaker notes and media out of a PowerPoint (`.pptx`). |
| `quickmap.html` | Reads GPS and time data from a folder of photos (JPG/HEIC), plots them on an editable map and exports KML, CSV or GeoJSON. |
| `download_shorthand.html` | Student-facing page with a bookmarklet that packages a Shorthand story (images and layout) into a single ZIP for assessment submission. |
| `ShorthandCaptureStaffTest.html` | Staff test build of Shorthand Capture: bookmarklets to copy a Shorthand story offline and screen-record it into one ZIP for assessment. |
| `Journalipsum.html` | Lorem ipsum, but journalese. Generates clichéd non-stories in different newsroom styles. |

## Installing moodle-feedback-helper

1. Unzip `moodle-feedback-helper-v3.zip`.
2. In Edge go to `edge://extensions` (or `chrome://extensions`) and turn on **Developer mode**.
3. Click **Load unpacked** and pick the `moodle-feedback-helper-v3` folder.
4. On Moodle, click the extension icon and choose your feedback folder. Matches appear on each student's grading page.

Folder access lapses when the browser restarts; reselect it from the extension icon.
