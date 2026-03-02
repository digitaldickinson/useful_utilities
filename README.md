# uni_utilities
A collection of odds and ends that may be helpful or help me manage day-to-day uni stuff.

- **mailmerge_to_customFilenameDoc.html** 
A simple HTML/JS page that will take a pre-formatted Word doc and a spreadsheet and create individually named Word docs like a mail merge. Like a mailmerg, it will also insert details such as student numbers, names, etc. into the Word doc, replacing a {{tag}}. I use this to generate named feedback files for student work. 

- **quickmap.html**
A small, single-page HTML file that reads GPS + time metadata from images in a folder and plots them on an interactive map. It supports JPG/JPEG and iPhone HEIC/HEIF, edit labels/descriptions and drag markers to correct locations, and can optionally draw a time-ordered path. Exports are aimed at real workflows: KML (with KML 2.2 TimeSpan for timeline support), CSV for tools like Datawrapper, and GeoJSON for modern mapping/GIS. Everything runs locally in your browser — no uploads, no server.
- **Note: This version doesn't work with Safari because it doesn't handle Folder picking** 
