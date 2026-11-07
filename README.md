# E-Commerce Customer Lifetime Value Preprocessing Pipeline

A case study in AI & ML: a pipeline that cleans raw e-commerce order data
and builds model-ready customer features (Recency, Frequency, Monetary, and more).

## Dataset
Online Retail, UCI Machine Learning Repository:
https://archive.ics.uci.edu/dataset/352/online+retail

## How to run
1. Download the dataset and place it in Google Drive (or upload it in Colab).
2. Open `clv_pipeline.ipynb` in Google Colab.
3. Choose Runtime, then Run all.

## Pipeline steps
1. Check data quality
2. Clean (missing IDs, duplicates, cancelled orders, invalid values)
3. Build features from orders before the cutoff date (2011-09-09)
4. Build the CLV target from orders after the cutoff
5. Cap outliers, scale (fit on training data only), split and save
