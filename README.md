# Mutual Fund NAV Prediction

## What this project does
Predicts the Net Asset Value (NAV) of mutual funds using their characteristics 
(fund type, category, AMC, minimum investment, average AUM, etc.) with regression models.

## Dataset
Mutual Fund NAV dataset containing details like Scheme Type, Scheme Category, AMC, 
Minimum Investment Amount, and Average AUM.

## Tools Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-learn, Jupyter Notebook

## What I did
- Cleaned missing values (median imputation for investment amount and AUM)
- Removed outliers from NAV using the IQR method
- Performed Exploratory Data Analysis (distribution plots, top AMCs, top scheme categories)
- Converted categorical variables into numeric form using one-hot encoding
- Scaled features and trained 4 models: Linear Regression, Lasso, Ridge, and ElasticNet
- Compared all models using R², MAE, and RMSE

## Results
| Model               | Test R² | MAE  | RMSE |
|---------------------|---------|------|------|
| Linear Regression    | 0.325   | 4.83 | 7.76 |
| Lasso Regression      | 0.229   | 5.20 | 8.29 |
| **Ridge Regression**  | **0.325** | **4.83** | **7.76** |
| ElasticNet Regression | 0.271   | 5.05 | 8.06 |

**Best Model:** Ridge Regression

## How to run it
Open `mutual_fund_nav_prediction.ipynb` in Jupyter Notebook or Google Colab and run all cells.
