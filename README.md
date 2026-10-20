# TallyDock

**A lightweight shipping-document review prototype.** Compare selected fields across an invoice, packing list, or transport document and flag values that need a human to verify.

## Try it

Once GitHub Pages finishes deploying, open:

https://gooroyeegar-design.github.io/TallyDock/

If the site is not available yet, check the [deployment workflow](https://github.com/gooroyeegar-design/TallyDock/actions).

## Current capabilities

- Load a fictional sample shipment to explore the workflow.
- Select two PDF, TXT, PNG, JPG, or WEBP files.
- Extract PDF text in the browser and use OCR for supported scanned PDFs/images when the third-party libraries load.
- Compare shipment reference, gross/net weight, carton quantity, goods description, and destination.
- Export a CSV comparison or a text review report; print/save a report as PDF.
- Review the original files yourself before acting on any flagged value.

## Important limitations

TallyDock is an **early prototype**, not production-ready logistics software and not a fully trained AI product. Its extraction and comparison are heuristic; OCR and field detection can miss or misread information. It does not determine which document is correct, perform customs clearance, connect to carriers, provide user accounts or team access, or offer a managed backend, audit trail, or service-level guarantee.

File extraction is designed to run in your browser. PDF.js and Tesseract.js are loaded from third-party CDNs, so file processing may not work if those services are unavailable. Do not use confidential, personal, commercially sensitive, or regulated shipment documents in this prototype. Use fictional/sample data until appropriate security, privacy, and reliability reviews are complete.

## Deployment

The GitHub Actions workflow in `.github/workflows/deploy.yml` publishes the repository to GitHub Pages on pushes to `main`. In repository settings, Pages should use **GitHub Actions** as the build and deployment source.

## Before commercial advertising

Do not advertise this prototype as an AI-powered, guaranteed, secure, or production-ready shipment compliance service. Before accepting real customer documents or paid users, add and test appropriate privacy/security controls, reliable document handling, accessibility and browser testing, monitoring, support/contact details, and clear commercial terms.
