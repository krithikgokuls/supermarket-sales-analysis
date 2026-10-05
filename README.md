# Supermarket Sales Analysis

## Project overview

This project analyzes 500 supermarket transactions across four branches to compare
product, category, branch, customer, payment, and rating performance. It validates
the source data, recalculates sales as `Quantity × Unit Price`, summarizes key
metrics, and plots comparisons to support practical business decisions.

## Dataset

- Source spreadsheet: [Supermarket Sales Dataset](https://docs.google.com/spreadsheets/d/1QIX__4VObHFMEXnRM2xJyXmB5JAB2peHrJcQ41_U9TE/edit?usp=sharing)
- Local CSV: `SUPER MARKET DATA - supermarket_sales_500_rows.csv`
- The notebook first looks for the CSV beside itself. If it is not found, it reads
  the CSV export from the source spreadsheet URL; internet access is required for
  that fallback.
- The analyzed file contains 500 rows and 13 columns, covering January 1 through
  July 1, 2026.

## Technologies

- Python 3.10+
- Jupyter Notebook
- pandas
- Matplotlib
- python-docx (only needed to regenerate the Word report)

## Setup and run

1. Install Python 3.10 or later.
2. Open a terminal in this project folder.
3. Install the required libraries:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Launch Jupyter:

   ```bash
   jupyter notebook
   ```

5. Open `YourName_SupermarketSalesAnalysis.ipynb` and choose **Run All**.
6. Keep `SUPER MARKET DATA - supermarket_sales_500_rows.csv` in the same folder,
   or allow the notebook to fetch the source CSV online.

Replace `YourName` in the notebook and report filenames with your own name before
submission.

## Key findings

- Total sales: **₹244,411.08**.
- Highest-sales product: **Cheese — ₹27,906.30**.
- Highest-sales branch: **Branch C (Mumbai) — ₹72,469.45**.
- Highest-sales category: **Beverages — ₹56,108.24**.
- Most-used payment method: **UPI — 127 transactions**.
- Average transaction sales: **₹488.82** for Members and **₹497.07** for Normal
  customers.
- Average customer rating: **3.99 / 5**.
- Source quality checks found no missing values or duplicate rows, and source
  Sales values matched Quantity × Unit Price to the nearest paisa.

## Deliverables

- `YourName_SupermarketSalesAnalysis.ipynb` — complete analysis and charts.
- `YourName_ProjectReport.docx` — formatted project report.
- `requirements.txt` — Python dependencies.
- `README.md` — project and run instructions.

The analysis is descriptive and based on the supplied sample. It identifies
associations and performance differences, not causes.
