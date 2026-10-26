# Postoperative PE and major bleeding dashboard

Interactive national results accompanying the manuscript on pulmonary embolism and major bleeding after primary elective hip and knee replacement in England, 2006 to 2025.

- **Live dashboard:** https://billyzhonguom.github.io/postop-pe-dashboard/
- **Updated:** 26 October 2026
- **Index admissions:** 1 January 2006 to 31 December 2025
- **Follow-up ends:** 30 April 2026
- **Cohorts:** 1,114,263 knee and 1,066,996 hip replacements
- **Analysis:** reviewed primary-replacement LRHE release `20261009`, result commit `46b88c3`

## Maintenance

This is a deployment mirror. Edit `dashboard/index.html` and run `dashboard/build_dashboard_data.py` in the parent `postoperative-pe-bleeding` project. The builder defaults to `results/lrhe_20261009/` and checks the analysis specification, cohort sizes, annual coverage and calendar periods. Copy the resulting `index.html` here and push to `main` to rebuild GitHub Pages.

The deployed page is self-contained apart from Chart.js and fonts. All numerical results are embedded from the reviewed aggregate tables. No patient-level data are included.

## Content

- National annual trends, 2006 to 2025, with in-hospital and post-discharge components
- Adjusted risks and odds ratios across four complete five-year periods, retaining 2020 and 2021
- Length of stay, annual procedure counts and proportion of events recorded after discharge
- Weekly and six-week first-event piecewise Poisson estimates, including the procedure-date sensitivity
- Post-discharge bleeding subtypes, with counts below 10 withheld before publication

Regional, ICB, Trust and provider benchmarking are outside this dashboard's scope.

Applied Health Research Unit, Nuffield Department of Population Health, University of Oxford.
