# Data Analyst Internship - Task 1

## Data Cleaning and Preprocessing

This project focuses on cleaning and preprocessing a raw dataset using Python and Pandas.

## Dataset

Dataset used:

Customer Personality Analysis

The dataset contains customer-related information such as education, marital status, income, customer date, and other customer attributes.

## Objective

The objective of this task is to clean and prepare the raw dataset by identifying and handling common data quality issues.

## Tools Used

- Python
- Pandas
- VS Code
- Git
- GitHub

## Data Cleaning Steps

### 1. Missing Values

Missing values were checked using Pandas.

The `Income` column contained 24 missing values.

The missing values were handled using the median value:

`51381.5`

After cleaning, there were 0 missing values in the Income column.

### 2. Duplicate Records

Duplicate rows were checked using Pandas.

Duplicate rows found:

`0`

### 3. Text Standardization

Text columns such as `Education` and `Marital_Status` were inspected and unnecessary leading/trailing spaces were removed.

### 4. Date Formatting

The `Dt_Customer` column was converted into a proper datetime format.

### 5. Column Names

Column names were standardized into lowercase format and spaces were replaced with underscores.

### 6. Outlier Checking

The `Income` column was checked for potential outliers using the IQR method.

Outliers were identified for investigation instead of being blindly removed.

### 7. Final Data Quality Check

The final dataset was checked for:

- Missing values
- Duplicate rows
- Data types
- Dataset shape

Final dataset shape:

`2240 rows × 29 columns`

Duplicate rows after cleaning:

`0`

## Project Structure

```text
Data_Analyst_Task_1/
│
├── dataset/
│   └── marketing_campaign.csv
│
├── cleaned_data/
│   └── marketing_campaign_cleaned.csv
│
├── venv/
│
├── load_data.py
├── test_pandas.py
├── cleaning_summary.txt
└── README.md