# Codefolio — Java Lab Report Studio

A single-page, browser-based tool for assembling Java lab reports and exporting them as PDF.

## Run locally
1. Extract the ZIP file.
2. Open `index.html` in a modern browser (Chrome or Edge recommended).
3. Edit the cover details, upload a cover image if you already have one, add Java code or text pages, then click **Export PDF**.

The PDF exporter uses jsPDF from a CDN, so an internet connection is needed for the direct **Export PDF** button. If the CDN is unavailable, the app falls back to your browser's print dialog; choose **Save as PDF**.

## Deploy to Vercel
This is a static website. Upload `index.html` to a GitHub repository and import that repository in Vercel. No build command is needed; set the output directory to `.`.

## Privacy
Report content is stored in this browser's local storage for autosave. It is not sent to a server by this app. The PDF library and web fonts are loaded from third-party CDNs.
