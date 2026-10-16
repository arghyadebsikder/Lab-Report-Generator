# Java Lab Report Studio

A single-page, browser-based editor for preparing Daffodil International University Java lab reports and exporting them as PDFs.

## Open locally

1. Download and extract the project ZIP.
2. Open `index.html` in Chrome or Edge.
3. Fill in the cover details or upload an existing cover page.
4. Add code and text pages. New pages are appended at the end of the document.
5. Export your finished report using **Export PDF**.

## Features

- DIU-styled cover page with editable report number, report title, course and student details, plus a submission-date field.
- Java source pages with syntax highlighting, an editable problem heading and file name, adjustable font family and font size, and dark/light editor themes.
- Long source code is automatically split over multiple PDF pages with rounded, padded code panels. The live preview remains a single A4 page and displays the estimated PDF page count.
- Page list shows the problem heading and Java file name; pages can be reordered, duplicated, or deleted.
- Separate text pages for algorithms, discussion, conclusions, and other written sections.
- Independent PDF code appearance toggle: enable dark code panels for screen-friendly reports or disable it for a light, printer-friendly PDF. Syntax colors keep readable contrast in both modes.
- Automatic saving to the current browser's local storage.
- Footer credit: “Made with ❤️ by Arghya”.

## PDF export

The export button uses jsPDF loaded from a CDN, so an internet connection is recommended. If the library is unavailable, the site opens the browser print dialog; choose **Save as PDF**.

All report data is stored in the local browser unless you upload or deploy the website elsewhere. Export a PDF backup before clearing browser storage.
