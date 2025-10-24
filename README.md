# Telco Customer Churn Analysis

This project analyzes the root causes for telco customer churn at a company, identifies key patterns, and recommends potential solutions to remediate this issue.

## Project Structure

```
Telco-Customer-Churn/
├── data/
│   ├── raw/                    # Raw, immutable data files
│   └── processed/              # Cleaned and processed data
├── notebooks/                  # Jupyter notebooks for analysis
├── src/                        # Source code modules
│   ├── __init__.py
│   ├── data_processing.py      # Data loading and preprocessing
│   ├── feature_engineering.py  # Feature creation and selection
│   ├── model_training.py       # Model training functions
│   ├── evaluation.py           # Model evaluation utilities
│   └── utils.py                # General utility functions
├── models/                     # Trained model artifacts
├── reports/                    # Generated reports and visualizations
│   └── figures/                # Plots and charts
├── tests/                      # Unit tests
├── requirements.txt            # Python dependencies
├── .gitignore                  # Git ignore file
└── README.md                   # This file
```

## Setup

1. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Explore the analysis in the Jupyter notebook:
```bash
jupyter notebook notebooks/telco_customer_churn.ipynb
```

## Data

The dataset contains customer information including:
- Customer demographics
- Services subscribed
- Account information
- Churn status 
