# Smart Document Renamer AI

A browser-based OCR tool for scanning and consistently renaming operational documents.

It accepts PDF and image files, reads identifying values with OCR, lets the user review each result, and exports the renamed files as a ZIP package or an Excel report.

## Features

- Drag-and-drop upload for PDF, JPG, JPEG, and PNG files
- OCR-based document number detection
- PDF text extraction with OCR fallback for scanned documents
- Supported document types: EDR, SI, SS, and DR
- Multi-pass digit voting and confidence/integrity checks
- Review table for detected values and manual corrections
- Batch export as a ZIP of renamed files
- Excel export for audit and reporting
- Runs fully in the browser—no server or document upload is required

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern desktop browser.
3. Choose the document type and year, add files, then click **Start Scan**.
4. Review the results before downloading the ZIP or Excel file.

## Technologies

- HTML, CSS, and vanilla JavaScript
- [Tesseract.js](https://github.com/naptha/tesseract.js) for OCR
- [PDF.js](https://mozilla.github.io/pdf.js/) for PDF processing
- JSZip, FileSaver.js, and SheetJS for exports

## Project background

This project was inspired by a practical workflow problem: document files often arrive with inconsistent or non-descriptive filenames, making organisation and retrieval slow. Smart Document Renamer AI automates the first pass while keeping a human review step before export.

Read the origin story on [LinkedIn](https://www.linkedin.com/pulse/how-one-conversation-inspired-me-build-ai-tool-jason-gil--g5eoc/).

## Notes

The app loads its libraries from public CDNs, so an internet connection is needed when opening it unless those dependencies are hosted locally.
