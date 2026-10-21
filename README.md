# customer-shopping

# Customer Spending Prediction (ShopSmart)

A machine learning web app that predicts a customer's **spend (in Rs.)** from their details.

**Live demo:** [Customer Spending App](https://customer-shopping-7wape4cwthvgptqhgiivdu.streamlit.app/)

## Dataset
- File: `ShopSmart_data.csv` (2,000 customers)
- Inputs: age, annual income, website visits, previous purchases, membership type, preferred category, city tier, discount used
- Target: customer spend

## Model
- Preprocessing: `OneHotEncoder` for categorical columns and `StandardScaler` for numeric columns, inside a `ColumnTransformer`
- Wrapped in a scikit-learn `Pipeline`
- Models compared: Linear Regression, Ridge, Lasso, KNN, Decision Tree, Random Forest
- Best model: Linear Regression with R² of 0.95
- Saved as `best_model_pipeline.pkl`

## Tech Used
Python, pandas, NumPy, scikit-learn, Seaborn, Streamlit

## How to Run
```
pip install -r requirements.txt
streamlit run app.py
```
