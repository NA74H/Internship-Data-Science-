# Sales Data Science Project

This repository contains a sales analytics notebook and dataset for performing exploratory data analysis (EDA), data cleaning, visualization, and a simple predictive model.

## Files

- `Untitled-1.ipynb` - Python notebook with the full analysis workflow.
- `Dataset_for_Data_Analytics_Sheet1.csv` - Sales dataset used in the notebook.

## Dataset Overview

The dataset contains sales order records with the following columns:

- `OrderID`
- `Date`
- `CustomerID`
- `Product`
- `Quantity`
- `UnitPrice`
- `ShippingAddress`
- `PaymentMethod`
- `OrderStatus`
- `TrackingNumber`
- `ItemsInCart`
- `CouponCode`
- `ReferralSource`
- `TotalPrice`

## What this project does

The notebook walks through common data analytics steps:

1. Data loading and initial inspection
2. Data cleaning and preprocessing
   - dropping missing values
   - normalizing categorical text values
   - removing duplicates
3. Exploratory data analysis (EDA)
   - summary statistics
   - distributions and descriptive metrics
4. Data visualization
   - product counts
   - sales by product
   - unit price distribution
   - top shipping locations by sales
   - correlation heatmap
5. Predictive modeling
   - train/test split
   - linear regression to predict `TotalPrice`
   - evaluation with R² and MAE
   - actual vs predicted visualization

## How to run

1. Open `Untitled-1.ipynb` in VS Code or Jupyter.
2. Make sure Python is installed.
3. Install necessary packages if needed:

```bash
pip install pandas seaborn matplotlib scikit-learn
```

4. Run the notebook cells in order.

## Notes

- The notebook is exploratory and may require further cleanup for production use.
- The current model demonstrates a simple regression baseline using sales-related features.
- You can extend the project with feature engineering, model tuning, or additional visualizations.
