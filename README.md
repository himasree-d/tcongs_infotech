# TCONGS Infotech — Website

A single-page marketing site with a hero section, process/revision-log showcase, and a scheduling call-to-action.

## Live Site

Once deployed via GitHub Pages: `https://himasree-d.github.io/tcongs_infotech/`

## Structure

```
tcongs_infotech/
├── index.html                  # Main page (markup + inline/linked CSS)
├── process-visual.mp4          # Compressed process/revision showcase video
└── README.md
```

## Features

- Responsive hero section
- Two-column process/revision log with a sticky reference video panel
- "Schedule Call" and related CTA buttons styled for both light and dark contexts
- Autoplaying, muted, looping video (optimized from a 47MB GIF down to ~834KB) for fast load times

## Running Locally

No build step required — it's static HTML/CSS/JS.

1. Clone the repo:
   ```
   git clone https://github.com/himasree-d/tcongs_infotech.git
   cd tcongs_infotech
   ```
2. Open `index.html` directly in a browser, or serve it locally:
   ```
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000`.

## Deployment

Deployed via **GitHub Pages** from the `main` branch (root folder). Any push to `main` automatically triggers a redeploy.

## Notes

- Keep `process-visual.mp4` and `process-visual-poster.jpg` in the same folder as `index.html` — the video reference in the markup expects relative paths.
- If replacing the process video in the future, compress it first (e.g. with `ffmpeg`) to keep page load fast.
