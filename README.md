# Logistics Data Analysis, Predictive Modeling and Optimization

This repository contains a complete logistics data analysis project developed as part of an internship program. The project is divided into three tasks that demonstrate the complete data analysis workflow, starting from data preprocessing and cleaning, followed by exploratory and advanced analysis, and finally predictive modeling and optimization.

The project uses a logistics delivery dataset containing information related to delivery distance, package weight, delivery time, expected delivery time, delivery cost, delivery partners, package types, vehicle types, delivery modes, regions, weather conditions, delays, and delivery status.

---

## Project Structure

```text
├── Delivery_Logistics.csv
├── cleaned_logistics_dataset.csv
├── preprocessing.ipynb
├── Advanced_Analysis.ipynb
├── Week_4_Predictive_Modeling_Logistics.ipynb
├── week3_visualizations/
│   ├── correlation_heatmap.png
│   ├── delay_status.png
│   ├── delivery_cost_distribution.png
│   ├── delivery_time_distribution.png
│   ├── distance_vs_cost.png
│   ├── partner_delivery_time.png
│   ├── vehicle_delivery_time.png
│   └── weather_delay_rate.png
└── README.md
```

---

# Week 2: Data Collection, Cleaning and Preprocessing

The first stage of the project focused on preparing the logistics dataset for analysis and machine learning.

The original dataset was loaded and examined to understand its structure, data types, missing values, duplicate records, and potential inconsistencies. Data cleaning and preprocessing techniques were then applied to improve the quality of the dataset.

### Key Activities

* Loaded the logistics delivery dataset.
* Examined dataset dimensions and column information.
* Checked for missing values.
* Identified and handled duplicate records.
* Performed data cleaning.
* Converted categorical variables into numerical format using encoding.
* Prepared the dataset for further analysis and machine learning.
* Generated a cleaned logistics dataset.

### Files

**Notebook:** `preprocessing.ipynb`

This notebook contains the complete code and detailed steps for:

1. Loading the dataset.
2. Exploring the dataset.
3. Checking data types.
4. Identifying missing values.
5. Detecting duplicates.
6. Cleaning the data.
7. Encoding categorical variables.
8. Saving the final cleaned dataset.

**Output Dataset:** `cleaned_logistics_dataset.csv`

The cleaned dataset produced during this task is used for the subsequent analysis and predictive modeling tasks.

---

# Week 3: Advanced Logistics Data Analysis

The second stage of the project focused on analyzing logistics performance and identifying patterns that influence delivery operations.

Exploratory and advanced data analysis techniques were used to understand the relationships between delivery time, distance, delivery cost, weather conditions, vehicle types, and delivery partners.

### Key Analysis Areas

#### 1. Weather and Delivery Delays

The relationship between weather conditions and delivery delays was analyzed to understand how different weather conditions affect logistics performance.

#### 2. Distance and Delivery Cost

The relationship between delivery distance and delivery cost was examined to identify how transportation distance influences operational costs.

#### 3. Delivery Time Performance

The distribution of delivery time was analyzed to understand the overall delivery performance of the logistics system.

#### 4. Delivery Partner Analysis

Different delivery partners were compared based on delivery time to identify variations in delivery performance.

#### 5. Vehicle Performance

The performance of different vehicle types was analyzed based on delivery time.

#### 6. Correlation Analysis

A correlation heatmap was created to identify relationships between numerical logistics variables.

### Visualizations

The following visualizations were generated:

* Delivery Time Distribution
* Delivery Cost Distribution
* Distance vs Delivery Cost
* Delivery Partner vs Delivery Time
* Vehicle Type vs Delivery Time
* Weather Condition and Delay Rate
* Delay Status Analysis
* Correlation Heatmap

### Files

**Notebook:** `Advanced_Analysis.ipynb`

The notebook contains the complete analysis process, Python code, observations, and interpretation of the results.

**Visualization Folder:** `week3_visualizations/`

This folder contains all graphs and visualizations generated during the Week 3 analysis.

---

# Week 4: Predictive Modeling and Optimization in Logistics Systems

The third stage of the project focused on developing machine learning models to predict delivery time and proposing optimization strategies based on the results.

The cleaned logistics dataset generated during Week 2 was used for predictive modeling.

### Problem Definition

The objective of this task was to predict:

`delivery_time_hours`

The prediction was performed using logistics-related features such as:

* Distance
* Package weight
* Expected delivery time
* Delivery rating
* Delivery cost
* Delivery partner
* Vehicle type
* Weather conditions
* Delivery delay status

### Machine Learning Models

Two regression models were developed and compared:

1. Linear Regression
2. Random Forest Regressor

The dataset was divided into training and testing sets using an 80:20 split.

### Model Evaluation

The models were evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

### Results

| Model                   |   MAE |  RMSE | R² Score |
| ----------------------- | ----: | ----: | -------: |
| Linear Regression       | 0.064 | 0.081 |    0.755 |
| Random Forest Regressor | 0.064 | 0.082 |    0.751 |

Linear Regression achieved slightly better overall performance and was selected as the preferred model.

The model achieved an R² score of approximately 0.755, meaning it was able to explain approximately 75.5% of the variation in delivery time.

### Feature Analysis

The most influential factors affecting delivery time were identified using the Linear Regression model coefficients.

The major factors included:

1. Delivery Cost
2. Stormy Weather
3. Distance
4. Rainy Weather
5. Delivery Delay Status
6. Foggy Weather
7. Expected Delivery Time

### Optimization Recommendations

Based on the predictive analysis, the following optimization strategies were proposed:

* Weather-based delivery planning.
* Route optimization to reduce delivery distance.
* Monitoring high-cost deliveries.
* Proactive delay management.
* Dynamic delivery scheduling.
* Efficient vehicle and resource allocation.

### Files

**Notebook:** `Week_4_Predictive_Modeling_Logistics.ipynb`

This notebook contains:

1. Data loading.
2. Feature and target selection.
3. Train-test splitting.
4. Linear Regression model training.
5. Random Forest model training.
6. Model evaluation.
7. Model comparison.
8. Feature importance analysis.
9. Visualization of results.
10. Optimization recommendations.

---

# Overall Workflow

The project follows a complete data science and machine learning workflow:

```text
Original Logistics Dataset
          ↓
Week 2: Data Cleaning and Preprocessing
          ↓
Cleaned Logistics Dataset
          ↓
Week 3: Exploratory and Advanced Analysis
          ↓
Insights and Visualizations
          ↓
Week 4: Predictive Modeling
          ↓
Model Evaluation and Comparison
          ↓
Feature Analysis
          ↓
Logistics Optimization Recommendations
```

---

# Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

---

# Dataset

The project uses the following dataset files:

* `Delivery_Logistics.csv` – Original logistics delivery dataset.
* `cleaned_logistics_dataset.csv` – Cleaned and preprocessed dataset used for advanced analysis and predictive modeling.

---

# Key Outcomes

Through the completion of these three tasks, the project demonstrates:

* Data collection and preprocessing.
* Data cleaning and transformation.
* Exploratory data analysis.
* Data visualization.
* Logistics performance analysis.
* Predictive modeling using machine learning.
* Model evaluation and comparison.
* Feature analysis.
* Data-driven logistics optimization strategies.

The project demonstrates how data analysis and machine learning can be applied to logistics systems to understand delivery performance, predict delivery time, identify important operational factors, and support data-driven decision-making.

---

## Author

**Bhavana B.**
Computer Science and Engineering
