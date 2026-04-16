# postop-pe-dashboard

Interactive dashboard accompanying the manuscript **"Post-discharge pulmonary embolism and major bleeding after elective hip and knee replacement in England: a self-controlled crossover study using national hospital data, 2006 to 2024."**

- **Live share link:** https://billyzhonguom.github.io/postop-pe-dashboard/
- **Manuscript citation:** reference [21]
- **Parent project repo:** https://github.com/BillyZhongUOM/postoperative-pe-bleeding

## How this repo is maintained

This is a **deployment mirror**. The authoritative source of the dashboard lives in the parent project repo at:

```
postoperative-pe-bleeding/dashboard/index.html
```

When the dashboard is updated there, the file is copied to `index.html` in this repo and pushed. GitHub Pages then rebuilds automatically on push to `main`.

Do **not** edit `index.html` directly in this repo — edits will be overwritten next time the parent project updates. All development happens in the parent repo's `dashboard/` folder, which also contains the Quarto source (`index.qmd` + `ahru.scss`) for the alternative Quarto-rendered version.

## Contents

- `index.html` — self-contained static dashboard (Leaflet + Chart.js + Mulish/Raleway fonts + embedded study data)

## Design

Visual identity follows the **AHRU / NDPH Oxford house style**:

- Primary navy `#051e41`
- Accent off-red `#f1290a`
- Warm off-white background `#F7F6F5`
- Typography: Mulish (body), Raleway (display)

## Disclosure controls

- ICBs with fewer than 10 events or fewer than 100 procedures in the selected period are automatically suppressed and hidden
- Trusts with known data gaps (Frimley Health Jun 2022 – Mar 2023; Shrewsbury and Telford Jul 2024 onwards) are flagged

## Attribution

Applied Health Research Unit, Nuffield Department of Population Health, University of Oxford.

This dashboard is a research tool for local benchmarking and is **not** a performance-ranking tool. Apparent differences between ICBs reflect case-mix, local coding practice, and service configuration as well as any genuine variation in outcomes.
