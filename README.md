# NLP Assignment 1

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![Pandas](https://img.shields.io/badge/pandas-data%20analysis-150458?logo=pandas)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-visualization-3f4f75?logo=plotly)](https://plotly.com/)

This repository contains the notebook for the NLP coursework. The notebook loads a hate speech dataset, extracts tweet text, cleans and normalizes the content, and performs exploratory analysis on the processed data.

## Overview

The notebook covers the full preprocessing flow used in the assignment:

- raw text extraction from the source CSV
- cleaning for URLs, mentions, HTML-like fragments, and noise
- tokenization and normalization helpers
- stopword handling and lightweight typo correction
- exploratory analysis with lengths, duplicates, and sample previews

## Files

- `NLP Assignment 1.ipynb` - main notebook
- `README.md` - repository overview
- `requirements.txt` - notebook dependencies
- `.gitignore` - notebook and Python cache exclusions

## Setup

Install the required packages before opening the notebook:

```bash
pip install -r requirements.txt
```

## How To Run

1. Open `NLP Assignment 1.ipynb` in Jupyter or VS Code.
2. Update the `raw_path` variable in the first code cell if your CSV file lives in a different location.
3. Run the cells from top to bottom to extract, clean, and analyze the dataset.

## What You Will See

- a preview of the extracted tweet text
- dataset shape, missing values, and duplicate counts
- tweet length summaries
- cleaned text outputs and preprocessing helpers
- sample exploratory analysis tables and plots

## Dataset

The notebook expects a local CSV file containing the raw hate speech dataset. In the notebook, the file path is stored in `raw_path`.

If you are using a different dataset location, update that variable before running the first data-loading cell.

## Notebook Flow

1. Load the raw text from the CSV file.
2. Clean and normalize the tweet content.
3. Build feature summaries such as character and word counts.
4. Inspect sample rows and preprocessing outputs.
5. Review the exploratory analysis tables and charts.

## Notes

- The notebook expects a local CSV file at the path defined in `raw_path`.
- If you move the dataset, update that path before running the notebook.

> **Note:** This notebook was written to run with a local dataset path. If the CSV is not on your machine, the first data-loading cell will need to be updated.

<div style="border-left:4px solid #059669; padding:12px; background:#ecfdf5; border-radius:6px; margin-top:12px;">
	<strong>Important:</strong> Make sure the source CSV file exists before running the notebook. The text extraction cell depends on that file path being valid.
</div>

<div style="border-left:4px solid #d97706; padding:12px; background:#fff7ed; border-radius:6px; margin-top:12px;">
	<strong>Warning:</strong> Some cells depend on the notebook being executed in order. Running later cells first may cause missing-variable errors.
</div>

## Helpful Setup Tips

- If you are working in a fresh environment, create a virtual environment before installing packages.
- If Plotly charts do not render inline, restart the kernel and run the notebook again from the top.
- If the dataset path is long, keep it in a raw string as shown in the notebook.
