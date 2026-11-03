# Kagaz Studio

A responsive, browser-first PDF and image utility suite. Files are processed in the user's browser; there is no upload endpoint in this static build.

## Install as a mobile app

Kagaz Studio includes a Progressive Web App (PWA) manifest and service worker. Serve it over HTTPS.

- **iPhone:** Open the site in Safari, tap Share, choose Add to Home Screen, keep Open as Web App enabled, then tap Add.
- **Android:** Open the site in Chrome, use the browser menu, and choose Install app or Add to Home screen.

The service worker caches the app shell for faster repeat visits and a basic offline fallback. PDF processing engines are loaded from public CDNs, so full PDF processing may still require an internet connection.

## Included tools

- Merge PDFs; split PDFs; remove pages; rotate pages; reverse page order; insert blank pages
- JPG/PNG/WebP to PDF; PDF to JPG/PNG; PDF to editable DOCX (text-only); PDF to TXT
- Compress PDF (rasterizes pages); compress/resize images
- Add page numbers; watermark; typed signature/approval text; edit PDF metadata
- Crop equal margins; grayscale conversion (rasterizes pages); add header/footer

## Important limitations

This is a static client-side utility, not a full Smallpdf/iLovePDF SaaS clone. OCR, secure password encryption/decryption, certificate-based digital signatures, cloud storage, accounts, billing, API access, and high-fidelity Office conversion are not included. Do not describe typed signature as a legally verifiable digital signature.

Some transformations rasterize pages, so text selection, links, and vector quality may be lost. Keep the original file when fidelity matters.

## Dependencies

- pdf-lib 1.17.1
- PDF.js 3.11.174
- JSZip 3.10.1

Libraries load from public CDNs at runtime.
