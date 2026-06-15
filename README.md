# House Price Tableau Dashboard and Data Story

This repository supports an academic Tableau visualisation project about house-price analysis and prediction reliability. The project uses a synthetic Kaggle-style house-price dataset to build a market overview dashboard, a model reliability dashboard, and a short Tableau data story.

The main idea is simple: a business user should be able to see how price changes across property features, then understand when model predictions are reliable enough to support review decisions.

## Business Problem

Property analysts often need a quick way to compare many records and identify which predicted prices need human review. A spreadsheet can hold the data, but it does not explain the story clearly. This Tableau project turns the prepared house-price data into dashboards that show market patterns, model accuracy, and review priorities.

## Dataset

The project is based on `house_price_50k.csv`, a synthetic house-price dataset associated with the Kaggle house price prediction project.

Dataset source:
https://www.kaggle.com/datasets/miadul/house-price-prediction-dataset

Important caveat: the dataset does not prove a real country, currency, transaction date, or official housing-market source. For that reason, the project uses `price units` instead of inventing a currency.

## Project Objectives

- Prepare Tableau-ready house-price data.
- Build a market overview dashboard using all 50,000 property records.
- Build a prediction reliability dashboard using the 10,000-row model holdout file.
- Show model metrics, review priority, and feature importance in a business-friendly way.
- Support the final academic report with real Tableau screenshots and validation evidence.

## Tableau Dashboards

The workbook contains two main dashboard areas and a seven-point story:

- Market overview: shows price patterns across location, income level, area, and selected filters.
- Prediction reliability: shows actual versus predicted price evidence, model quality, and review-priority examples.
- Data story: guides the reader from market context to model reliability and recommendations.

Final screenshots are stored in `screenshots/`. The screenshot source map is stored in `docs/SCREENSHOT_SOURCE_MAP.md`.

## Final Results

Best model: Ridge Regression

- MAE: 15,954 price units
- RMSE: 19,941 price units
- R-squared: 0.9981
- Cross-validation RMSE: 20,018 price units

The strongest practical message is that area is the main price driver in this synthetic dataset. Location and income level add useful segmentation, while the prediction dashboard helps identify records that deserve closer human review.

## Repository Structure

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

## How To Reproduce

1. Install the Python requirements.

```bash
pip install -r requirements.txt
```

2. Open the packaged workbook in Tableau Desktop.

```text
tableau/workbook/house_price_tableau_dashboard.twbx
```

3. Review the final dashboard and story screenshots in `screenshots/`.

## Files Included

- `data/raw/house_price_50k.csv`: original project dataset.
- `data/processed/house_price_tableau.csv`: Tableau market dashboard file.
- `data/derived/model_predictions_tableau.csv`: model holdout prediction evidence.
- `data/derived/model_metrics_tableau.csv`: model performance metrics.
- `data/derived/feature_importance_tableau.csv`: feature importance evidence.
- `tableau/workbook/`: Tableau workbook files.
- `screenshots/`: final dashboard and story screenshots.
- `evidence/`: workbook, screenshot, and report-readiness notes.

## Files Not Included

The academic Word report and PDF are intentionally not included in this GitHub repository. They are kept in the private local submission package because GitHub is being used here for reproducibility and supporting evidence, not as the formal report submission folder.

## Known Limitations

- The dataset is synthetic and should not be treated as live housing-market data.
- Price values are described as `price units` because no verified currency is provided.
- Tableau screenshots are static evidence of the final dashboard/story states.
- The model results are suitable for coursework demonstration, not commercial property valuation.

## GitHub Repository Information

Repository name: `HousePriceTableaud`

## Academic Disclaimer

This repository supports an academic Machine Learning Visualisation and Data Analytics assessment. It is designed for reproducibility, review, and transparent evidence. It is not a commercial valuation tool.

