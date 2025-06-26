# VIRENNA QA Redirect Page

This GitHub Pages site provides a trusted, accessible, and secure redirect for accessing critical QA medical documents.

## How it works

- This page immediately redirects users to an encrypted ProtonDrive document.
- It includes a fallback card with:
  - QR Code
  - "Open QA Report" button
  - Optional SHA-256 checksum for integrity check
- Fully static: No JavaScript required.

## How to update

1. Clone this repository.
2. Edit `index.html`:
   - Replace the ProtonDrive URL in the `<meta>` and QR/image/button.
   - Update the SHA-256 hash block if available.
3. Push to `main` branch.

## QR Code Generator

You can generate a new QR code using:

https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=YOUR_LINK

**Never generate a QR that links to `qa.virenna.org` itself – this causes infinite loops. Always use the final ProtonDrive URL.**

## Accessibility Features

- High contrast
- Focus outlines
- ARIA labels
- Responsive layout
- Dark Mode support

## License

MIT – but must only be used for validated VIRENNA QA redirects.
