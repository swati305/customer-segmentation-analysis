# Customer Segmentation & Behavioral Analysis

**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Power BI  
**Project type:** Portfolio project using synthetic data

## Overview
This project generates a synthetic customer and transaction dataset, explores purchase behavior, calculates Recency–Frequency–Monetary (RFM) metrics, applies K-Means clustering, and exports segment-level data for Power BI.

> **Data note:** All records are synthetic and generated for demonstration. They do not represent real customers or actual company performance. Revenue figures reflect randomly generated prices in the dataset.

## Workflow
1. Generate 5,000 synthetic customer records and 25,000 transactions.
2. Check data quality and explore customer and category patterns.
3. Calculate RFM metrics for customers with at least one transaction.
4. Log-transform and standardize RFM features.
5. Compare cluster counts using the elbow method and silhouette score.
6. Fit a four-cluster K-Means model and profile the customer segments.
7. Explore category preferences and export CSVs for Power BI.

## Customer segments
- High-Value Frequent
- Recent High-Value
- Regular Customers
- Low-Value Inactive

Segment names are assigned from the observed cluster profiles and should be rechecked if the data or model settings change.

## How to run
1. Install dependencies: `pip install -r requirements.txt`
2. Open `customer_segmentation_github_ready.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Run all cells from top to bottom.
4. CSV files will be saved to the notebook's current working directory for use in Power BI.

## Exported files
- `customers.csv`
- `transactions.csv`
- `customer_segments.csv`
- `transactions_with_segments.csv`
- `segment_summary.csv`
- `top_categories_by_segment.csv`

## Limitations
The data is synthetic and transactions are randomly generated. Results demonstrate an analysis workflow and should not be interpreted as real-world customer behavior. For production use, validate the method with an appropriately licensed real dataset and business context.
