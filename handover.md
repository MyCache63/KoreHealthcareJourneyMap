# KoreHealthcareJourneyMap — Handover

## Current State
Interactive HTML patient journey map is **complete and deployed**.

- Faithfully reproduces Slide 9 from `AI for Healthcare_Enablement_March 2026.pptx`
- 21 journey step boxes across 4 phases (Before the Visit, After the Visit, Patient Discharge, Recovery & Beyond)
- Each box shows a hover popup with plausible Kore.ai use case content (description, bullet points, key metric badge)
- Layout uses absolute positioning matching exact slide coordinates (EMU-to-% conversion)
- Colors extracted from PPTX theme: white (Patient), light blue #57A0E3 (Member), gradient (Patient & Member), dark blue #0C5EAB (Payer)
- SVG connecting lines and timeline dots match the slide's tree/branch structure
- Light blue gradient background matching the slide's watercolor background image

## Deployment
- **GitHub repo**: https://github.com/MyCache63/KoreHealthcareJourneyMap
- **Live site**: https://mycache63.github.io/KoreHealthcareJourneyMap/
- GitHub Pages deployed via Actions workflow (`.github/workflows/pages.yml`)
- Deployment confirmed successful

## Files
- `index.html` — The complete interactive journey map (single self-contained HTML file, no external dependencies)
- `bg.png` — Extracted background image from PPTX (not currently used; CSS gradient used instead)
- `.github/workflows/pages.yml` — GitHub Pages deployment workflow
- `CLAUDE.md` — Project instructions
- `handover.md` — This file

## Key Decisions
- Hover popups (not click) — Michael's preference
- Popup content is plausible Kore.ai messaging, not sourced from actual Kore.ai materials
- PowerPoint/Google Slides cannot support hover interactivity — recommendation is to present the HTML directly in a browser tab during presentations (fullscreen with F11)

## Build Status
- No build step needed — it's a static HTML file
- Opens directly in any browser
- Hosted live on GitHub Pages

## Next Steps (if any)
- Add a fullscreen/presentation mode button if desired
- Refine popup content with actual Kore.ai messaging if available
- Could add click-to-pin tooltip behavior for touch devices
- Michael may want to adjust specific box text or colors after reviewing
