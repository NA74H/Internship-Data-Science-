# Sales Data Science Project

This repository contains a sales data science pipeline built around a sales order dataset. It includes exploratory data analysis (EDA), visualization, preprocessing, and a baseline predictive model.

## Repository structure

- `Untitled-1.ipynb` - interactive Jupyter notebook with the full EDA and modeling workflow.
- `Dataset_for_Data_Analytics_Sheet1.csv` - sales dataset used for analysis.
- `eda.py` - script that generates EDA plots and saves them into `eda_outputs/`.
- `modeling.py` - script that trains a baseline regression model and saves outputs into `model_outputs/`.
- `requirements.txt` - Python packages required for the scripts.
- `eda_outputs/` - generated exploratory plots.
- `model_outputs/` - trained model artifacts and metrics.

## Dataset overview

The dataset includes sales order-level features such as:

- `OrderID`
- `Date`
- `CustomerID`
- `Product`
- `Quantity`
- `UnitPrice`
- `TotalPrice`
- `ShippingAddress`
- `PaymentMethod`
- `OrderStatus`
- `TrackingNumber`
- `ItemsInCart`
- `CouponCode`
- `ReferralSource`

## What this project does

### Notebook workflow (`Untitled-1.ipynb`)
- Load and inspect the dataset
- Clean and preprocess data
  - drop missing values
  - normalize categorical text fields
  - remove duplicate records
- Perform exploratory data analysis
  - summary statistics
  - distributions and category counts
- Visualize data
  - product counts
  - sales by product
  - price distributions
  - top shipping locations
  - correlation heatmap
- Build a baseline predictive model
  - train/test split
  - linear regression on `TotalPrice`
  - evaluation with R² and MAE
  - actual vs predicted plot

### Scripted workflow
- `eda.py` generates plots and saves them into `eda_outputs/`.
- `modeling.py` trains a `RandomForestRegressor` pipeline and saves:
  - `model.joblib`
  - `metrics.json`
  - `feature_importances.png` (when available)

## Setup and usage

1. Create a Python environment if needed.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook with Jupyter or VS Code.

4. Or run the scripts directly:

```bash
python eda.py
python modeling.py
```

## Optional notebook dependencies

The notebook also uses Plotly for interactive visualizations. If you want to run the Plotly cells, install:

```bash
pip install plotly
```

## Output locations

- `eda_outputs/` - saved EDA charts from `eda.py`
- `model_outputs/` - trained model and evaluation metrics from `modeling.py`

## Next steps

- improve feature engineering
- add model cross-validation
- try alternate targets like classification or segmentation
- expand visualizations for business insights
