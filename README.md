# Earthquake Building Damage Prediction

Predicts **mean building damage** from earthquakes using **XGBoost**.

## Dataset
- File: `15.eq_building_damage.csv`
- Target: `meandamage`
- Cleaning steps:
  - Dropped `Unnamed: 0` if present
  - Fixed `year_built` (>2025 → 1925)
  - One-hot encoded `struct_typ` & `occ_type`

## Requirements
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
Run
python earthquake_damage_prediction.py
Workflow

Load & clean data

Encode categorical features

Train-test split (80-20)

Train XGBoost Regressor

Evaluate with MAE & R²

Visualize results:

Heatmap

Actual vs Predicted plot

Feature Importance chart

Example Output
Mean Absolute Error: 0.124
R-squared: 0.87
Author

Arangi Srivalleswari




