# Bank Marketing Dataset - Exploratory Data Analysis (EDA)

## Overview
This project focuses on analyzing the **Bank Marketing Dataset** to understand patterns in customer behavior and campaign effectiveness. The dataset consists of customer demographics, banking details, and marketing interaction data. The goal is to extract meaningful insights using **data visualization** and **statistical analysis**.

## Dataset
The dataset contains the following key attributes:
- **age**: Age of the customer
- **job**: Type of job (e.g., admin, technician, entrepreneur, etc.)
- **marital**: Marital status (e.g., single, married, divorced)
- **education**: Level of education
- **credit_default**: Whether the customer has defaulted on credit (yes/no)
- **housing**: Whether the customer has a housing loan (yes/no)
- **loan**: Whether the customer has a personal loan (yes/no)
- **campaign**: Number of contacts performed during this campaign
- **pdays**: Number of days since the client was last contacted
- **previous**: Number of times the client was contacted before the current campaign
- **poutcome**: Outcome of the previous marketing campaign
- **duration**: Last contact duration in seconds
- **y**: Target variable (whether the client subscribed to a term deposit)

## Data Preprocessing
- **Handling Missing Values**: Replaced missing values using mode and median imputation.
- **Removing Duplicates**: Identified and dropped duplicate records.
- **Outlier Detection**: Handled outliers in `age`, `duration`, and `pdays`.
- **Feature Engineering**:
  - Renamed columns for clarity.
  - Reordered dataset columns.
  - Dropped unnecessary columns (`month`, `day_of_week`, `contact`, `previous`).
- **Encoding**:
  - Applied **One-Hot Encoding** for categorical variables.
  - Used **Label Encoding** for the target variable (`y`).

## Exploratory Data Analysis (EDA)
- **Histograms & Box Plots**: Analyzed distributions and outliers.
- **Scatter Plots & Bar Plots**: Explored relationships between features.
- **Correlation Heatmaps**: Identified highly correlated variables.
- **Class Imbalance Analysis**: Measured distribution of the target variable (`y`).

## Results
- The dataset had **class imbalance**, with a majority of customers **not subscribing** to term deposits.
- Features like **duration**, **previous campaign outcome**, and **number of contacts** significantly impact customer subscription rates.
- Certain features (`emp.var.rate`, `euribor3m`) were dropped due to low correlation with the target variable.

## Requirements
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## How to Run
1. Download the dataset using:
!kaggle datasets download henriqueyamahata/bank-marketing !unzip /content/bank-marketing.zip

2. Run the `eda_bank_marketing_dataset_.py` script to perform data analysis.

3. Visualizations and insights will be displayed in the output.

## Future Improvements
- Apply **Machine Learning Models** for customer prediction.
- Perform **feature selection** to improve data quality.
- Use **clustering techniques** to group customer behavior patterns.

## Acknowledgments
Dataset sourced from Kaggle. This project is for educational purposes.

نسخ
تحرير

