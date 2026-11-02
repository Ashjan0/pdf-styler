# PDF Styler

A browser tool to restyle PDF slides: change colours, add page numbers and your own text, remove a watermark, and print several slides on one A4 page.
Everything runs in the browser (pdf.js + jsPDF). Your PDF is never uploaded.

## Features
- Upload or drag & drop any PDF, with a live preview of any slide
- Slide background colour (presets + custom) and slide text colour
- Cover a watermark: corner presets or draw the area on the preview
- Page numbers and custom text (name, roll no., college) with font, size (pt), colour and position
- A4 layouts: 1, 2, 3, 4, 6 or 9 slides per page, auto/portrait/landscape, gap, border, paper colour
- Website themes: Dark, Light, Ocean, Forest, Rose, or your own custom colours (saved in the browser)
- Export quality: Standard / High / Max

## Run locally
Open `index.html` in a modern browser. No install needed (internet is needed once to load pdf.js and jsPDF from a CDN).

## Publish on GitHub Pages
1. Create a repository and upload `index.html` and `README.md`
2. Settings → Pages → Deploy from a branch → `main` / root
3. In `index.html`, set `const GITHUB = '...'` to your profile URL to show the GitHub link

## How it works
Each slide is rendered to a canvas with pdf.js. The tool then covers watermark areas (blending the surrounding colours), recolours the background and text pixels, draws numbers and text, places slides on A4 sheets, and builds the new PDF with jsPDF.

## Known limits
- Output pages are images, so text can't be selected or copied.
- Background/text recolouring is pixel based: best on slides with a plain background. Photos can shift slightly.
- Watermark cover works best on plain or softly shaded backgrounds.

## Ideas for later
- Keep selectable text (vector output)
- Merge / split PDFs, logo stamp

Built by Ashraf.
