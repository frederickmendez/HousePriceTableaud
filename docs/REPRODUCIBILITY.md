# Reproducibility Notes

This repository is designed to support review of the Tableau dashboard and data story.

## Local Checks

Install the Python requirements if you want to inspect the CSV files locally:

```bash
pip install -r requirements.txt
```

Useful manual checks:

- confirm the report DOCX/PDF files are not inside the GitHub folder;
- confirm row counts match the expected data grain;
- confirm model metrics match the verified Ridge Regression evidence;
- confirm the Tableau workbook files are present;
- confirm screenshots are real PNG files with readable dimensions.

## Tableau Review

Open the packaged workbook in Tableau Desktop:

```text
tableau/workbook/house_price_tableau_dashboard.twbx
```

The final dashboard and story evidence is available in:

```text
screenshots/dashboards/
screenshots/story/
```

## Report Files

The academic Word and PDF reports are kept outside GitHub in the private submission package. They are intentionally excluded from this repository.

