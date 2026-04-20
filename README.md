# uni_utilities
A collection of odds and ends that may be helpful or help me manage day-to-day uni stuff.

<img width="816" height="742" alt="image" src="https://github.com/user-attachments/assets/4a4a7e1f-fadf-4e62-9a29-d37f2c14b7c9" />

- **mailmerge_to_customFilenameDoc.html** 
A simple HTML/JS page that will take a pre-formatted Word doc and a spreadsheet and create individually named Word docs like a mail merge. Like a mailmerge, it will also insert details such as student numbers, names, etc. into the Word doc, replacing any {{tag}} style content. I use this to quickly generate named feedback files ready to mark student work.

<img width="1209" height="715" alt="image" src="https://github.com/user-attachments/assets/29e83efd-e5ef-4560-9b99-d5b0f6f0695d" />

- **moodles.html** 
A simple HTML/JS page designed to make creating and uploading feedback files easier in Moodle. It takes a zip file of Moodle submissions, strips out submission IDs and names. You can also side-load a Moodle Grading sheet (CSV) to add more data (optional). This can then be merged with a feedback template in a doc format.  The app will look for {{TAGS}} to replace based on the submission ID and data from the CSV. Then it will export personalised feedback templates with the correct filename to work with the bulk upload function in Moodle. No uploads, etc. It's all local (apart from access to CDN/Libs). This version is tuned to my Uni's version of Moodle. File naming conventions may vary depending on your version of Moodle.  

<img width="1002" height="764" alt="image" src="https://github.com/user-attachments/assets/b412a949-3ffa-4af2-b1d6-0713d8c16bd1" />

- **powerpuller.html** 
A simple HTML/JS page that will take a PowerPoint presentation (PPTX) and extract text, notes and media.  It was originally designed to quickly grab speaker notes. But I thought it would be useful to quickly be able to pull apart a PPT file if you wanted to update or repurpose. 

<img width="2160" height="1303" alt="image" src="https://github.com/user-attachments/assets/2a1135a9-a0f6-4932-8df8-197ed8d23bd0" />

- **quickmap.html**
A small, single-page HTML file that reads GPS + time metadata from images in a folder and plots them on an interactive map. It supports JPG/JPEG and iPhone HEIC/HEIF, edit labels/descriptions and drag markers to correct locations, and can optionally draw a time-ordered path. Exports are aimed at real workflows: KML (with KML 2.2 TimeSpan for timeline support), CSV for tools like Datawrapper, and GeoJSON for modern mapping/GIS. Everything runs locally in your browser — no uploads, no server!

<img width="1269" height="745" alt="Screenshot 2026-04-20 at 19 19 15" src="https://github.com/user-attachments/assets/77243ab3-e23e-4242-a037-e044b7e32aa8" />


* **moodle-feedback-helper** *(Microsoft Edge extension)*
  A browser extension that sits alongside Moodle's assignment grading interface and matches files from a local feedback folder to the student currently being graded. When you open a grading page, it reads the student's name from the page, scans your chosen folder for any file containing that name (fuzzy — handles `Student_Name.docx`, `Student Name.docx`, `2394729_Name_Student.docx`, `Student.docx` etc.), and displays matches in a floating panel. Files can be dragged directly into Moodle's upload area or uploaded programmatically with one click. Cuts out the window-switching and manual hunting that comes with Moodle ordering submissions by time rather than alphabetically. The selected folder persists across student pages without re-selecting.

  **Installation**
  1. Download `moodle-feedback-helper.zip` and unzip it
  2. In Microsoft Edge, go to `edge://extensions`
  3. Enable **Developer mode** (toggle, top right)
  4. Click **Load unpacked** and select the unzipped `moodle-feedback-helper` folder
  5. The extension icon will appear in your toolbar

  **Usage**
  1. Navigate to your Moodle instance and click the extension icon
  2. Click **Select Feedback Folder** and choose the folder containing your feedback files
  3. Open any student's grading page — the panel appears automatically
  4. Matched files appear in the panel; drag them onto Moodle's upload area, or click **Upload →** to attempt automatic injection
  5. The extension icon also shows which student is currently being graded

  > Folder access permissions lapse when the browser restarts — just click the extension icon and reselect the folder (it remembers the name). The programmatic **Upload →** button targets common Moodle file manager selectors; if it reports the drop zone isn't found, dragging will still work. Built for Edge, but should load in Chrome under developer mode.
