# 🏠 Building Damage Prediction During an Earthquake  

## 📌 Project Overview  
This project predicts **earthquake-induced mean building damage** using the **XGBoost regression algorithm**.  

It covers **data preprocessing, feature encoding, model training, evaluation, and visualization**.  
Its application helps in **disaster planning** by estimating the **structural vulnerability** of buildings.  

---

## ✨ Key Features  
- Loads and cleans the **earthquake building damage dataset**  
- Converts categorical features (`struct_typ`, `occ_type`) using **one-hot encoding**  
- Trains an **XGBoost regression model** to predict **mean building damage** (`meandamage`)  
- Evaluates model performance using:  
  - **Mean Absolute Error (MAE)**  
  - **R-squared (R²)**  
- Provides visualizations:  
  - Correlation heatmap  
  - Actual vs. Predicted scatter plot  
  - Top 10 feature importance chart  

---

## 📂 Example Dataset Fields  

| Feature      | Description |
|--------------|-------------|
| **struct_typ**   | Building structural type (e.g., URM, C4, S1, W1) |
| **occ_type**     | Occupancy type (e.g., RES1, COM1, AGR1, IND1) |
| **year_built**   | Year the building was constructed |
| **no_stories**   | Number of floors/stories |
| **magnitude**    | Earthquake magnitude |
| **distance**     | Distance from the epicenter |
| **meandamage**   | Mean damage value (label for regression) |

👉 All features are used for regression, with categorical ones encoded and cleaned before training.  

---

## 🔎 Methods Summary  
1. **Clean** raw earthquake/building damage data  
2. **Encode** categorical variables (`struct_typ`, `occ_type`) using one-hot encoding  
3. **Train** the XGBoost regression model  
4. **Evaluate** with MAE and R² Score  
5. **Visualize** correlations, predictions, and feature importances  

---

## 📊 Results  
- **Mean Absolute Error (MAE):** `0.12` *(example value)*  
- **R² Score:** `0.87` *(example value)*  
- **Key Findings:**  
  - Structural type (`struct_typ`) and occupancy type (`occ_type`) are major predictors.  
  - Earthquake magnitude and distance significantly affect building damage.  
  - Feature importance analysis highlights construction year and number of stories as critical factors.  

---

## 🚀 Future Scope  
- Hyperparameter tuning for improved accuracy  
- Add geospatial/seismic features (soil type, coordinates, shaking intensity)  
- Include regional building codes & construction practices  
- Deploy as an **interactive app** (Flask/Streamlit)  
- Explore deep learning and ensemble models  

---

## 📜 License  
This project is licensed under the **MIT License**.  

