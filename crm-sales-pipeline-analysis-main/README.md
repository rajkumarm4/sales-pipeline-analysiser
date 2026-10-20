# CRM Sales Pipeline Analysis

This repository contains a CRM sales pipeline analysis project with cleaned sales data, preprocessing code, a Tableau dashboard, and a final analysis report.

## Project Overview

The project analyzes CRM sales opportunities to understand sales performance, deal outcomes, pipeline value, sales cycle timing, products, accounts, and regional team performance.

## Repository Structure

```text
.
├── README.md
├── requirements.txt
├── .gitignore
├── corrected-files/
│   ├── data/
│   │   ├── accounts.csv
│   │   ├── accounts_clean.csv
│   │   ├── products.csv
│   │   ├── products_clean.csv
│   │   ├── sales_pipeline.csv
│   │   ├── sales_pipeline_clean.csv
│   │   ├── sales_teams.csv
│   │   └── sales_teams_clean.csv
│   ├── dashboard/
│   │   └── CRM Sales_Dashboard.twbx
│   ├── notebooks/
│   │   └── Preprocessing_step.ipynb
│   └── report/
│       └── CRM Sales Pipeline Analysis.pdf
└── original-files/
    └── original uploaded files preserved as received
```

## Key Files

- `corrected-files/notebooks/Preprocessing_step.ipynb`: Python preprocessing notebook.
- `corrected-files/data/accounts_clean.csv`: cleaned account data.
- `corrected-files/data/products_clean.csv`: cleaned product data.
- `corrected-files/data/sales_pipeline_clean.csv`: cleaned CRM opportunity data with calculated fields.
- `corrected-files/data/sales_teams_clean.csv`: cleaned sales team data.
- `corrected-files/dashboard/CRM Sales_Dashboard.twbx`: Tableau packaged dashboard.
- `corrected-files/report/CRM Sales Pipeline Analysis.pdf`: final project report.

## Data Tables

The project uses four main CRM tables:

- `accounts`: company account details, including sector, revenue, employees, location, and parent company information.
- `products`: product names, series, and sales prices.
- `sales_pipeline`: sales opportunity records, including sales agent, product, account, deal stage, dates, and deal value.
- `sales_teams`: sales agent, manager, and regional office mapping.

## Analysis Workflow

1. Load raw CRM datasets.
2. Fill missing account and opportunity values.
3. Convert date columns to date/time format.
4. Create calculated fields such as:
   - `sales_cycle_days`
   - `is_won`
   - `year`
5. Export cleaned CSV files.
6. Build a Tableau dashboard from the cleaned data.
7. Summarize insights in the final PDF report.

## File Notes

The original files are preserved in `original-files/`.

During repository preparation, several uploaded files appeared to have mismatched filenames or extensions. To make the project easier to use, corrected copies were added under `corrected-files/`.

Examples:

- The uploaded `products.csv` appears to contain the Jupyter notebook.
- The uploaded `CRM Sales_Dashboard.twbx` appears to contain the PDF report.
- The uploaded `data_dictionary.csv` appears to contain the Tableau packaged workbook.
- Several CSV-style files appear to be shifted by filename.

Use `corrected-files/` for normal project review, and `original-files/` if you need to verify the exact uploaded attachments.

## Requirements

Install Python dependencies with:

```bash
pip install -r requirements.txt
```

Main libraries:

- pandas
- jupyter

## How to Use

1. Open `corrected-files/notebooks/Preprocessing_step.ipynb`.
2. Run the notebook to reproduce cleaned CSV outputs.
3. Open `corrected-files/dashboard/CRM Sales_Dashboard.twbx` in Tableau Desktop or Tableau Reader.
4. Review `corrected-files/report/CRM Sales Pipeline Analysis.pdf` for the final analysis summary.

## Suggested Repository Name

`crm-sales-pipeline-analysis`
