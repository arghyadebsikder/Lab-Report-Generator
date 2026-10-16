# Codefolio — DIU Java Lab Report Studio

A browser-based editor for assembling Java programming assignments and lab reports into a polished A4 PDF.

## Features

- DIU-inspired white cover page based on the sample design, with the university wordmark, faint crest watermark, and a thin page border.
- Default cover heading: **Lab Report - 02**.
- Default report topic: **Summer -26 & Fall - 25 OOP Mid Term Question Solution Using JAVA**. Both the report number and topic are editable. The cover does not use an “Experiment Name” label.
- Optional upload of an existing cover page (PNG, JPG, or WebP).
- Java source pages with an editable problem heading and editable filename. Every new code page starts as `Main.java`.
- Adjustable code font family (Monospace, Sans serif, Serif) and font size (6–12 pt), reflected in the live preview and PDF export.
- Separate text pages for algorithms, discussions, output explanations, and conclusions.
- Page selection, move up/down, duplicate, and delete controls. The cover remains fixed as page one.
- Live A4 preview and browser-local autosave when browser storage is available.

## Open locally

1. Extract the ZIP.
2. Open `index.html` in Chrome or Edge.
3. Edit the cover details, paste Java source code, and add, move, duplicate, or delete pages.
4. Select **Export PDF**.

The DIU wordmark and watermark are embedded in `index.html`, so the website preview does not depend on image files. The `assets/` folder keeps the original logo artwork used to build the cover design.

The PDF export library is loaded from a CDN, so an internet connection is needed for the direct **Export PDF** button. If the browser blocks local storage for a `file://` page, the top status will show **Autosave unavailable**; your current edits still work, but export a PDF before closing the tab. For browser autosave, open the folder with a local web server (such as VS Code Live Server) or deploy it to Vercel.

## Deploy to Vercel

1. Upload the contents of this project folder to a GitHub repository.
2. Import the repository into Vercel.
3. Choose the static/Other framework preset, with no build command and no output directory required.
4. Deploy. The entry point is `index.html`.

## Notes

- Autosaved report data remains in the current browser only; it does not automatically sync between computers or browsers.
- Inspect the exported PDF before submitting, especially if the code contains very long lines or the report uses many pages.
