# Boston House Price Prediction 🏡

## 📌 Project Description

This project uses machine learning to predict house prices in Boston. I test multiple models and optimize performance using feature engineering and hyperparameter tuning.

## 📂 Dataset

- **Boston House Prices** (Kaggle) https://www.kaggle.com/datasets/vikrishnan/boston-house-prices
- The dataset contains house prices and variables such as crime rate, number of rooms, taxes, etc.

## 🛠️ Technologies and Tools

- **Python 🐍**
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost

## 🔬 Feature Engineering
To improve the model, I created new features and transformed existing data:
- **TAX_per_ROOM** = `TAX` (property tax) divided by `RM` (number of rooms)  
- **AGE_per_DIS** = `AGE` (building age) divided by `DIS` (distance to jobs)  
- **LSTAT_squared** = `LSTAT` (percentage of low-income families) **squared**  
- **log_CRIM** = Log transformation of `CRIM` (crime rate per area)  

## 🔧 Model Optimization
- **Hyperparameter tuning with Grid Search**  
- **Tested Random Forest and XGBoost**  
- **Chose XGBoost as the best model after Feature Engineering**  

## 🏆 Models and Results

| Model                      | MAE  | MSE   | R² Score |
| -------------------------- | ---- | ----- | -------- |
| **Linear Regression**      | 3.96 | 35.75 | 0.56     |
| **Random Forest**          | 2.89 | 26.42 | 0.68     |
| **Standard XGBoost**       | 2.84 | 22.67 | 0.72     |
| **XGBoost + Feature Eng.** | 2.68 | 19.60 | 0.76     |

XGBoost with Feature Engineering provided **the best performance**, with the lowest error and highest R² score.

## 🚀 How to Run the Project

1. **Install necessary packages**
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn xgboost
   ```
2. **Download the dataset**
3. **Run the Python script or open Jupyter Notebook**

## 📊 What Did I Learn?

- **Feature Engineering improved performance**
- **XGBoost was the best model**
- **Hyperparameter tuning helped find optimal values**

## 💎 Contact

If you have any questions, contact Julie Jansen at julie_emmy_95@hotmail.com or www.linkedin.com/in/julie-jansen-a73232138.

