# Kagaz Studio

A responsive, browser-first PDF and image utility suite. Files are processed in the user's browser; there is no upload endpoint in this static build.

## Included tools

- Merge PDFs
- Split PDFs (extract pages, ranges, or individual pages)
- Remove pages
- Rotate pages
- Reverse page order
- Insert blank pages
- JPG/PNG/WebP to PDF
- PDF to JPG/PNG
- PDF to editable DOCX (text-only; layout/images/tables are not preserved)
- PDF to TXT (selectable text only)
- Compress PDF (rasterizes pages; selectable text is lost)
- Compress/resize images with target-size option
- Add page numbers
- Add watermark
- Add typed signature/approval text
- Edit PDF metadata
- Crop equal margins
- Convert PDF to grayscale (rasterizes pages)
- Add header/footer and page count

## Run locally

Open `index.html` in a modern browser with an internet connection. PDF libraries are loaded from public CDNs. For best results, serve the folder over localhost or deploy it as a static site.

## Important limitations

This is a static client-side utility, not a full Smallpdf/iLovePDF SaaS clone. OCR for scanned documents, password encryption/decryption, certificate-based digital signatures, cloud storage, accounts, billing, API access, and high-fidelity Office conversion are not included. Those features need dedicated libraries and/or a secure backend. Do not describe the typed signature tool as a legally verifiable digital signature.

Some transformations intentionally rasterize pages (PDF compression and grayscale conversion), so text search, selection, links, and vector quality may be lost. Keep the original file when fidelity matters.

## Dependencies

- pdf-lib 1.17.1
- PDF.js 3.11.174
- JSZip 3.10.1

Libraries are loaded from cdnjs at runtime.
