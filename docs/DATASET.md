# Dataset Notes

The project uses `house_price_50k.csv` from the Kaggle house price prediction dataset:

https://www.kaggle.com/datasets/miadul/house-price-prediction-dataset

The source is used as synthetic coursework data. It does not verify a real country, currency, transaction date, or official housing-market provenance. The project therefore describes the target as `price` measured in unspecified `price units`.

## Files

| File | Purpose |
| --- | --- |
| `data/raw/house_price_50k.csv` | Original dataset file kept for traceability. |
| `data/processed/house_price_tableau.csv` | Full 50,000-row market file for Tableau. |
| `data/derived/model_predictions_tableau.csv` | 10,000-row model holdout prediction file. |
| `data/derived/model_metrics_tableau.csv` | Ridge, Linear Regression, and Random Forest model metrics. |
| `data/derived/feature_importance_tableau.csv` | Feature importance evidence used in the dashboard/story. |
| `data/derived/location_income_summary.csv` | Aggregated market summary for dashboard use. |

## Model Metrics

The best model evidence is Ridge Regression:

- MAE: 15,954 price units
- RMSE: 19,941 price units
- R-squared: 0.9981
- Cross-validation RMSE: 20,018 price units

