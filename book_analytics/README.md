# Book Market Analytics: Books to Scrape (Data Science 500)
https://github.com/Tintsw01/book-market-analytics/edit/main/book_analytics/README.md
[Link Text Here](https://github.com/Tintsw01/book-market-analytics/edit/main/book_analytics/README.md)

## Run it
1. `pip install -r requirements.txt` (Python 3.9+, internet connection needed for the first run).
2. `jupyter notebook Book_Market_Analytics.ipynb`, then **Kernel > Restart & Run All**.
3. First run scrapes all 1,000 books (about 3-5 minutes) and saves `data/books_raw.csv`. Re-runs reuse it; set `FORCE_SCRAPE = True` to scrape again.

## Outputs created by the notebook
- `data/books_raw.csv`: raw scraped data. `data/books_clean.csv`: **final cleaned dataset (deliverable 2)**.
- `figures/`: 8 PNG charts to paste into your report.
- `results/summary.json`, `model_metrics.csv`, `model_coefficients.csv`: every number you need for the report.

## Deliverables checklist
1. Jupyter notebook: `Book_Market_Analytics.ipynb`. Run it and keep the saved outputs.
2. Final dataset: `data/books_clean.csv`.
3. Report: complete `REPORT_TEMPLATE.md` using your own results, then export to PDF (Times New Roman 12, 1.5 spacing, Harvard referencing, cover page, signed declaration).

Before submitting, write the two interpretation sections in the notebook (after the charts and after the model) in your own words.
