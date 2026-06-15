# Tableau Evidence Readiness

Generated: 2026-06-15T08:18:18+02:00

Status: `READY_FOR_SUBMISSION_ZIP`

## Summary

- Workbook ready: `True`
- Screenshots ready: `True`
- Readiness evidence ready: `True`
- Final report ready: `True`

## Workbook Checks

- `.twb`: exists, parses as XML, and contains seven story points.
- `.twbx`: exists and passes zip integrity checks.
- Packaged CSVs are included in the workbook package.

## Screenshot Checks

- Six dashboard screenshots are present in `screenshots/dashboards/`.
- Seven Tableau story screenshots are present in `screenshots/story/`.
- Final screenshot dimensions meet the expected quality threshold.

## Report Handling

The final DOCX and PDF report files are intentionally excluded from this GitHub repository. They are stored in the private local submission package.

## Caveats

- The dataset is synthetic.
- Price values use unspecified `price units`.
- The market dashboard uses the 50,000-row market file.
- The prediction reliability evidence uses the 10,000-row model holdout file.

