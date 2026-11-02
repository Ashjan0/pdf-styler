# Ashraf PDF Styler

A small browser tool to **change the background** of PDF slides and **add slide numbers**.
Everything runs in the browser (pdf.js + jsPDF) — your PDF is never uploaded anywhere.

## Features
- Upload / drag & drop any PDF
- Background colour presets + custom colour picker
- Slide numbers: position, format (`3`, `3 / 23`, `Page 3`, `Slide 3`), colour, size, start number
- Live preview of any slide
- Download the styled PDF (quality selectable)

## Run locally
Just open `index.html` in your browser. No install needed.

## Publish on GitHub Pages (free)
1. GitHub par naya repository banao, e.g. `pdf-styler`
2. `index.html` aur `README.md` upload karo
3. **Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save**
4. 1–2 minute baad site live hogi: `https://YOUR-USERNAME.github.io/pdf-styler/`

> `index.html` me `YOUR-USERNAME` ko apne GitHub username se replace kar do (2 jagah: header aur footer).

## Tech
HTML, CSS, vanilla JavaScript, [pdf.js](https://mozilla.github.io/pdf.js/), [jsPDF](https://github.com/parallax/jsPDF)

## Known limits
- Output pages are images, so text in the new PDF can't be selected/copied.
- Works best with dark/colour backgrounds when the slide text is white.

## Roadmap ideas
- Light-theme mode with automatic text recolouring
- Keep selectable text (vector output)
- Footer / header text, logo stamp
- Merge / split PDFs

Built by Ashraf.
