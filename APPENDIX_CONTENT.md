# Appendix Content For Report

This text is prepared for manual insertion into the final report appendix.

## Appendix A: Dataset Information

The project uses the `house_price_50k.csv` dataset from the Kaggle house price prediction project:

https://www.kaggle.com/datasets/miadul/house-price-prediction-dataset

The dataset contains 50,000 property records and 19 original columns. The target variable is `price`. The project treats the data as synthetic because the source does not verify a real country, currency, transaction date, or official housing-market provenance. For this reason, the report and dashboard use the term `price units`.

The Tableau market file is `data/processed/house_price_tableau.csv` and keeps the full 50,000-row market view. The prediction evidence file is `data/derived/model_predictions_tableau.csv` and contains 10,000 holdout prediction records.

## Appendix B: Repository Structure

```text
HousePriceTableaud_Sanitized_Final/
├── README.md
├── .gitignore
├── requirements.txt
├── FILE_STRUCTURE.md
├── APPENDIX_CONTENT.md
├── data/
│   ├── raw/
│   ├── processed/
│   └── derived/
├── tableau/
│   └── workbook/
├── screenshots/
│   ├── dashboards/
│   └── story/
├── evidence/
└── docs/
```

The repository is intentionally focused on reproducibility and supporting evidence. Internal drafts, old remediation folders, rendered page images, temporary exports, and private report files are not included.

## Appendix C: GitHub Repository Information

GitHub repository:

https://github.com/<owner>/HousePriceTableaud

The repository includes the Tableau workbook, supporting CSV files, final screenshots, validation evidence, and documentation. The academic Word report and PDF are not included in GitHub; they are kept in the private submission package.

## Appendix D: Tableau Workbook Information

Workbook files:

- `tableau/workbook/house_price_tableau_dashboard.twb`
- `tableau/workbook/house_price_tableau_dashboard.twbx`

The packaged workbook was validated with Tableau Desktop 2026.1 evidence. The workbook contains a market overview, prediction reliability views, and a seven-point Tableau story. The readiness evidence records that the `.twb` parses as XML, the `.twbx` package passes zip integrity checks, and the story contains seven story points.

## Appendix E: Supporting Files

Supporting evidence files include:

- `screenshots/dashboards/`: six final dashboard screenshots.
- `screenshots/story/`: seven final Tableau story screenshots.
- `evidence/TABLEAU_EVIDENCE_READINESS.md`: workbook validation summary.
- `evidence/TABLEAU_EVIDENCE_READINESS.md`: readiness summary.
- `evidence/official_screenshot_contact_sheet_2026-06-15.png`: screenshot contact sheet.

