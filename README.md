# Customer-data-cleaning-python
Python data cleaning and preprocessing project demonstrating missing-value treatment, outlier handling, categorical encoding, and numerical standardization.

# 🧹 Customer Data Cleaning & Preprocessing using Python

## 📌 Project Overview : - https://colab.research.google.com/drive/1-KJLnxpGcI7EUqdS0FCiPM0Sqp4xKvct?usp=sharing

This project demonstrates an end-to-end data cleaning and preprocessing workflow using Python.

The objective was to transform a raw customer dataset containing missing values, potential outliers, and categorical variables into a clean and analysis-ready dataset.

The project demonstrates common data preprocessing techniques used in Data Analyst and Data Science workflows.

---

## 🎯 Objectives

- Identify missing values
- Handle missing numerical and categorical data
- Check for duplicate records
- Detect and treat outliers
- Encode categorical variables
- Standardize numerical features
- Validate the cleaned dataset
- Export the processed dataset as CSV

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

---

## 📊 Dataset

The original dataset contained:

- **15 customer records**
- **6 columns**

### Original Columns

| Column | Description |
|---|---|
| Customer_ID | Unique customer identifier |
| Age | Customer age |
| Gender | Customer gender |
| City | Customer city |
| Annual_Income | Annual customer income |
| Purchase_Count | Number of purchases |

---

## 🧹 Data Cleaning Process

### 1. Missing Value Detection

Missing values were identified using Pandas:

```python
df.isnull().sum()


2. Missing Value Treatment

Numerical missing values were replaced using the median.

Categorical missing values were replaced using the mode.

3. Duplicate Check

Duplicate records were checked using:

df.duplicated().sum()

The final dataset contained:

0 duplicate rows

4. Outlier Detection

The Interquartile Range (IQR) method was used to identify potential outliers.

An unrealistic age value was identified and corrected using the median.

5. Categorical Encoding

The Gender column was converted into numerical features using one-hot encoding.

Gender
   ↓
Gender_Female
Gender_Male
6. Numerical Standardization

The following numerical features were standardized using StandardScaler:

Age
Annual_Income
Purchase_Count

Customer_ID was intentionally excluded because it is an identifier rather than an analytical feature.

📈 Before vs After
Metric	Before	After
Rows	15	15
Columns	6	7
Missing Values	Present	0
Duplicate Rows	Checked	0
Gender Encoding	Text	Numerical
Numerical Scaling	Not applied	Standardized

The increase from 6 to 7 columns is due to converting the Gender categorical variable into two one-hot encoded columns.

📋 Final Data Quality Report
Rows: 15
Columns: 7
Missing values: 0
Duplicate rows: 0

The resulting dataset is clean and ready for further analysis or machine learning workflows.

📁 Project Structure
customer-data-cleaning-python/
│
├── customer_data_cleaning_preprocessing.ipynb
├── customer_data_cleaned.csv
├── data_cleaning_summary.csv
└── README.md
▶️ How to Run
Google Colab

Open the notebook in Google Colab and execute the cells sequentially.

Local Environment

Install the required libraries:

pip install pandas numpy scikit-learn matplotlib

Then open:

customer_data_cleaning_preprocessing.ipynb

using Jupyter Notebook or JupyterLab.

💡 Skills Demonstrated
Data Cleaning
Data Preprocessing
Python
Pandas
NumPy
Missing Value Handling
Median Imputation
Mode Imputation
Outlier Detection
IQR Method
One-Hot Encoding
Feature Standardization
Data Validation
CSV Export
📌 Project Outcome

The project transformed a raw customer dataset into a clean and structured dataset with:

0 missing values
0 duplicate records
Corrected outlier
Encoded categorical variables
Standardized numerical features

The final dataset is ready for downstream data analysis.

👨‍💻 Author

Arya Marale

Data Analyst | Python | SQL | Power BI | Excel
