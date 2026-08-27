#  Logistics Data Collection, Cleaning and Preprocessing

## Project Overview

This project focuses on collecting, cleaning, and preprocessing a logistics delivery dataset using Python. The objective is to prepare raw logistics data for further analysis and machine learning applications.

The preprocessing pipeline includes data exploration, data type correction, missing value analysis, duplicate detection, outlier detection, numerical normalization, categorical encoding, and final dataset validation.

## Objectives

- Load and explore a logistics dataset using Pandas.
- Identify numerical and categorical variables.
- Check for missing values.
- Check for duplicate records.
- Correct inappropriate data types.
- Detect outliers using the IQR method.
- Normalize numerical variables using Min-Max Scaling.
- Encode categorical variables using One-Hot Encoding.
- Validate and save the final cleaned dataset.

## Dataset

The logistics dataset contains **25,000 delivery records** and **15 original variables**.

The dataset includes information related to:

- Delivery partners
- Package types
- Vehicle types
- Delivery modes
- Regions
- Weather conditions
- Delivery distances
- Package weights
- Delivery times
- Expected delivery times
- Delay status
- Delivery status
- Delivery ratings
- Delivery costs

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Visual Studio Code

## Preprocessing Steps

### 1. Data Loading

The dataset was loaded using Pandas.

```python
df = pd.read_csv("logistics_dataset.csv")
```

### 2. Data Exploration

The dataset structure was examined using:

```python
df.head()
df.shape
df.columns
df.dtypes
```

### 3. Data Type Correction

The `delivery_time_hours` and `expected_time_hours` columns were initially interpreted as timestamp-like values. They were converted into numerical values for analysis.

### 4. Missing Value Analysis

```python
df.isnull().sum()
```

**Result:** 0 missing values.

### 5. Duplicate Detection

```python
df.duplicated().sum()
```

**Result:** 0 duplicate records.

### 6. Outlier Detection

The IQR method was used for `distance_km`.

- **Q1:** 75.9 km
- **Q3:** 224.9 km
- **IQR:** 149.0 km
- **Lower Bound:** -147.6 km
- **Upper Bound:** 448.4 km
- **Outliers:** 0

### 7. Numerical Normalization

Min-Max Scaling was applied to:

`distance_km`, `package_weight_kg`, `delivery_time_hours`, `expected_time_hours`, `delivery_rating`, and `delivery_cost`.

All values were scaled between **0 and 1**.

### 8. Categorical Encoding

One-Hot Encoding was applied to:

`delivery_partner`, `package_type`, `vehicle_type`, `delivery_mode`, `region`, `weather_condition`, `delayed`, and `delivery_status`.

### 9. Final Validation

- **Rows:** 25,000
- **Columns:** 43
- **Missing Values:** 0
- **Duplicate Records:** 0
- **Distance Outliers:** 0

## Project Structure

```text
Week2_Logistics_Preprocessing/
├── preprocessing.py
├── logistics_dataset.csv
├── cleaned_logistics_dataset.csv
└── README.md
```

## Output

The cleaned dataset was saved as `cleaned_logistics_dataset.csv` and is ready for further logistics analysis and machine-learning applications.

## Key Findings

| Metric | Result |
|---|---:|
| Original Rows | 25,000 |
| Original Columns | 15 |
| Final Rows | 25,000 |
| Final Columns | 43 |
| Missing Values | 0 |
| Duplicate Records | 0 |
| Distance Outliers | 0 |
| Normalization | Completed |
| Categorical Encoding | Completed |

## Conclusion

The logistics dataset was successfully cleaned and preprocessed using Python. Data types were corrected, missing and duplicate values were checked, outliers were analyzed, numerical data was normalized, and categorical data was encoded. The final dataset is ready for further logistics analytics.
