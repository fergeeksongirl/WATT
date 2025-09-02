# WATTs — Workforce Assessment for Transition & Talent

Single‑file, client‑side demo that helps talent assess skills and discover energy career pathways.
This repository contains the **stable v13.1 build**.

> **Privacy by design**: No accounts, no tracking, no server. Everything runs in the browser. Printing and email use the user’s local client (e.g., system print dialog, `mailto:`).

---

## Contents

- `index.html` 
- `legal/` — license files (code + assets), security, support and contributing docs

> _All content herein is sourced from the project’s file set provided by the client. No external sources are used unless explicitly noted._

---

## What is WATTs?

WATTs helps users self‑assess their skills via **Core / Established / Emerging** sections and produces a concise recommendation (General Level, Primary Focus, Upgrades).  


### Key Features

- **Single page**: HTML + CSS + JS in one file for easy hosting.
- **Accessible by default**: Keyboard friendly, ARIA labeling for dialogs and status, device‑agnostic wording.
- **Print‑friendly**: Users can export their results to paper or PDF.
- **Private**: No data leaves the browser.

---

## Quick Start

1. Download this repository (or the HTML files only).
2. Open one of the HTML files directly in your browser:
   - `index.html`
3. Use the pathway selector to run the standard assessment.
4. Print or save as PDF from your browser’s print dialog.

> Tip: The app works offline. You can double‑click the HTML file to open it locally.

---

## Project Structure

```
/
├─ index.html
└─ legal/
   ├─ LICENSE   (Code license: MIT)
   ├─ ASSETS_LICENSE.md    (Non‑code assets policy)
   ├─ CONTRIBUTING.md
   ├─ SECURITY.md
   ├─ SUPPORT.md
   └─ CODE_OF_CONDUCT.md
```

---

## Accessibility Notes

- Device‑agnostic language (avoid positional cues like “top right”).  
- Descriptive ALT text and ARIA labels on interactive elements (e.g., modal `aria-labelledby`, status `aria-live`).  
- Mobile: Likert labels wrap; results/summary tables are scrollable and use fixed layout to prevent overflow.

---

## Development

Because this is a single‑file app, “development” means editing the HTML (and embedded CSS/JS).

- **Data** lives in a client‑side JSON structure inside the script (`DATA`, plus `FOUNDATION` and optional `CROSSWALK` for Explorer Mode).
- **Builders**: `buildLikert()` renders each section; `collect()` gathers responses; `computeResults()` populates KPIs and recommendations.
  
### Local Testing

- Open the HTML file in Chrome/Edge/Firefox/Safari (desktop + mobile).  
- Verify: pathway select, overview modal, section flow, calculate results, print, explore another.  
- For mobile, confirm labels wrap and tables don’t overflow.

### Style & Comments

- Keep functional code unchanged when making documentation edits.  
- Use **HTML comments** for section markers and **JS block comments** for region maps.

---

## Versioning

See **docs/WATTs_Changelog.md**. This repo includes:
- `v13.1` (stable)

---

## License

- **Code** is licensed under **MIT** (see `legal/LICENSE`).  
- **Non‑code assets** (text content, datasets, images, PDFs) are **not** covered by the MIT grant and remain the property of their respective owners (see `legal/ASSETS_LICENSE.md`).

---

## Support

If you encounter issues, please check **legal/SUPPORT.md** for contact details and response 


**Build:** 2025-08-31 14:14:28Z
