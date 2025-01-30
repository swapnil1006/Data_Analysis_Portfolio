# Week 1: Data Cleaning and Preprocessing

## Project: Customer Churn Prediction Dataset Cleaning

### Objective
The goal of this project is to clean and preprocess the Telco Customer Churn dataset for predictive modeling.

### Dataset
- Source: [Telco Customer Churn Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)
- Description: The dataset contains customer information for a telecommunications company, including demographics, account details, and churn status.

### Steps Taken
1. **Handled Missing Values**:
   - Replaced empty strings in `TotalCharges` with NaN.
   - Filled missing values with the median.
2. **Detected and Treated Outliers**:
   - Used the IQR method to remove outliers in `MonthlyCharges`.
3. **Encoded Categorical Variables**:
   - Applied one-hot encoding to convert categorical variables into numerical format.
4. **Normalized Features**:
   - Scaled `MonthlyCharges` and `TotalCharges` using Min-Max scaling.

### Output
- Cleaned dataset saved as `cleaned_telco_churn.csv`.
- Full cleaning steps documented in the Jupyter Notebook: [data_cleaning.ipynb](data_cleaning.ipynb).

### Tools and Libraries Used
- Python Libraries:
  - `pandas`: Data manipulation
  - `numpy`: Numerical computations
  - `matplotlib` and `seaborn`: Data visualization
  - `scikit-learn`: Feature scaling