# Automobile Data Exploratory Data Analysis (EDA)

## Objective
Leverage Python and visualization tools to clean, transform, and analyze automobile data to uncover actionable insights about vehicle pricing, brand trends, and performance metrics[cite: 1].

## Problem Statement
The automobile dataset contains raw vehicle specification and pricing data with missing values, inconsistencies, and skewed distributions that limit direct analysis[cite: 1]. This project focuses on data cleaning, exploratory analysis, and visualization to understand how factors such as brand, engine size, fuel type, and efficiency influence car pricing and performance[cite: 1].

## Dataset Overview
The dataset consists of 205 records and 15 features encompassing vehicle specifications, performance metrics, and pricing[cite: 1]. 

**Key Features:**
*   **Identifiers:** `car_id` (Unique identifier)[cite: 1]
*   **Categorical:** `make` (brand), `fuel-type`, `body-style`, `drive-wheels`, `engine-location`, `engine-type`[cite: 1]
*   **Numerical:** `symboling`, `normalized-losses`, `width`, `height`, `engine-size`, `horsepower`, `city-mpg`, `highway-mpg`, `price`, `curb_weight`, `num_doors`[cite: 1]

## Technologies & Libraries Used
*   **Language:** Python[cite: 1]
*   **Data Manipulation:** Pandas, NumPy[cite: 1]
*   **Data Visualization:** Matplotlib, Seaborn[cite: 1]
*   **Preprocessing:** Scikit-learn (`StandardScaler`, `LabelEncoder`)[cite: 1]

## Project Workflow
1.  **Data Loading & Initial Inspection:** Imported the raw `Automobile_data.csv` dataset using Pandas and examined data types, dimensions, and descriptive statistics[cite: 1].
2.  **Data Quality Assessment:** Isolated categorical and numerical columns to evaluate unique values and identify structural inconsistencies[cite: 1].
3.  **Missing Value Treatment:** Replaced missing placeholder values (e.g., `?`) with `NaN`, then imputed `normalized-losses` and `horsepower` using appropriate fill values and statistical medians[cite: 1].
4.  **Data Type Correction:** Converted relevant object data types to integers to facilitate accurate mathematical operations[cite: 1].
5.  **Duplicate Removal:** Audited the dataset for duplicate rows to ensure data integrity[cite: 1].
6.  **Outlier Detection & Handling:** Applied the Interquartile Range (IQR) method to detect outliers across all numerical features and utilized value clipping to prevent skewed distributions from impacting the analysis[cite: 1].
7.  **Feature Scaling:** Standardized key numerical features (such as `price`, `engine-size`, `city-mpg`, and `highway-mpg`) using `StandardScaler` to align data distributions[cite: 1].
8.  **Categorical Encoding:** Transformed categorical string variables into machine-readable numeric formats using `LabelEncoder`[cite: 1].
9.  **Feature Engineering:** Created derived metrics, specifically the `price/horsepower` ratio, to extract deeper analytical value regarding cost-to-performance[cite: 1].

## How to Use
1. Clone this repository to your local machine.
2. Ensure you have the required analytical libraries installed (`pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`).
3. Open `Template Automobile_EDA.ipynb` in Jupyter Notebook or your preferred Python IDE[cite: 1].
4. Run the cells sequentially to reproduce the end-to-end data cleaning, preprocessing, and engineering pipeline[cite: 1].

---
**Author:** Arya Gupta
