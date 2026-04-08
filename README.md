# Transformational AI: Analyzing Ecommerce Large Datasets for Machine Learning

## Project Overview

This project analyzes two Amazon Reviews 2023 datasets (Electronics) sourced from Hugging Face to perform data transformation, analysis, and visualization. The goal is to prepare top-quality datasets for model fine-tuning and customer satisfaction analysis at Transformational AI.

## What This Project Does

1. **Environment Setup** — Installs and configures required Python libraries in a Jupyter Notebook environment.
2. **Data Loading** — Downloads 100 samples each from the Amazon Reviews and Metadata datasets using Hugging Face's `datasets` library with streaming.
3. **Data Exploration** — Inspects DataFrames using `.head()`, `.dtypes`, `.info()`, and `.columns` from `pandas`.
4. **Data Cleaning** — Filters products by average rating (≥ 4.5), valid price, and non-null title, producing a cleaned dataset of top products.
5. **Data Export** — Saves cleaned data as `top_products.csv` and `top_products.parquet`.
6. **Data Visualization** — Creates histograms and scatterplots using `seaborn` and `matplotlib` to visualize price distributions and rating trends.
7. **Further Filtering** — Narrows down to highly rated products (≥ 4.7) and generates a final dashboard for business and ML teams.

## Requirements

- Python 3.13+
- Jupyter Notebook

### Python Packages

Listed in `requirements.txt`:

- `datasets`
- `pandas`
- `matplotlib`
- `seaborn`
- `pyarrow`

Install with:

```bash
pip install -r requirements.txt
```

## Project Structure

```
├── readme.md                          # This file
├── requirements.txt                   # Python dependencies
├── Udacity - PCEP Project.ipynb       # Main project notebook
├── top_products.csv                   # Exported cleaned dataset (CSV)
├── top_products.parquet               # Exported cleaned dataset (Parquet)
└── user_inputs.txt                    # Reflection question responses
```

## How to Run

1. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook "Udacity - PCEP Project.ipynb"
   ```
4. Run all cells sequentially. Some cells require manual input for reflection questions.

## Deliverables

- `Udacity - PCEP Project.ipynb` — Completed notebook with cell outputs
- `user_inputs.txt` — Answers to all reflection questions
- `top_products.csv` — Cleaned dataset in CSV format
- `top_products.parquet` — Cleaned dataset in Parquet format
