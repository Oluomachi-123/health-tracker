# 🏃‍♂️ Personal Health Tracker

A small, frontend-only web app to track daily water intake, sleep hours, and exercise minutes. Stores data in the browser (LocalStorage), provides a BMI calculator, and visualizes progress with charts.
HELO
---

## Quick Start

1. Open `index.html` in your web browser (double-click or drag into a browser window).
2. Use the navigation buttons to switch between pages:
   - Home — app overview
   - Add Entry — log today's (or any date's) water, sleep, and exercise
   - Records — view all saved entries
   - Summary — see averages and days tracked
   - BMI — calculate body mass index and category
   - Charts — generate interactive progress charts

No server or installation is required. The app works offline and stores data locally in your browser.

## Features

- Add, view, and persist daily health records (water, sleep, exercise) using LocalStorage.
- BMI calculator with simple category output (Underweight, Normal, Overweight, Obese).
- Interactive line charts (Chart.js) for visualizing trends over time.
- Mobile-friendly, responsive layout and simple navigation with Font Awesome icons.

## Files

- `index.html` — single-file web app containing HTML, CSS, and JavaScript. This is the only file you need to run the app.
- `PROJECT_PLAN.md` — project plan and notes (requirements, design, and usage instructions).

## How it works (short)

The app is frontend-only. Data model is stored as a JSON object in `localStorage` under the key `healthRecords`.

Main functions:

- `addEntry()` — saves water, sleep, and exercise values for a date.
- `displayRecords()` — renders a table of saved entries.
- `displaySummary()` — computes averages and days tracked.
- `calculateBMI()` — computes BMI from height (cm) and weight (kg).
- `drawCharts()` — renders Chart.js line charts for each metric.

## Usage notes & tips

- Data persists per-browser profile. Clearing browser storage or using a different browser/profile will not show the same records.
- Dates are stored in ISO format (`YYYY-MM-DD`) and are sorted when displayed.
- Input validation is minimal: the BMI calculator checks for non-zero height/weight; entries with empty numeric fields will be treated as 0.

## Known limitations

- No user accounts or server-side storage (data is local only).
- Minimal validation and no undo/delete entry UI (you can clear LocalStorage from browser devtools to reset data).
- Single-file structure means styles and scripts are inline — consider splitting for larger projects.

## Suggested next steps (small improvements)

1. Add edit/delete for individual records.
2. Add CSV export/import so users can back up or import data.
3. Improve input validation and show friendly error messages.
4. Split CSS/JS into separate files and add simple build tooling (optional).
5. Add unit tests for the JS logic (if the app is refactored into modules).

## License & Contribution

This repository doesn't include a license file. If you want to share or open-source it, add a `LICENSE` file. "MIT" is a good permissive default; if you want, I can add one for you.

Contributions:

- Prefer small, focused changes. If you want me to implement a feature, tell me which one and I'll create a draft change.
- For a local workflow: create a branch, make changes, and open a PR. Since this is a simple single-file app, small refactors or adding export/import are safe first changes.

---

Generated from `index.html` and `PROJECT_PLAN.md`.
