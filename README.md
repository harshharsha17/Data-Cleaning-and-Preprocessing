# Data Cleaning and Preprocessing - Customer Personality Analysis

## Overview
This project is part of the **Data Analyst Internship Task 1**.  
The objective was to **clean and prepare a raw dataset** containing customer marketing data for further analysis. The dataset used is the **Customer Personality Analysis dataset** from Kaggle.

---

## Dataset
- **Original File:** `marketing_campaign.csv`  
- **Rows:** 2240  
- **Columns:** 29  
- Contains customer demographic and spending information including `Education`, `Marital_Status`, `Income`, `Dt_Customer`, and product purchase data.

---

## Data Cleaning Steps

1. **Handled Missing Values**
   - Found 24 missing values in the `Income` column.
   - Filled missing values with the **median** of the column to avoid bias from outliers.

2. **Removed Duplicates**
   - Checked for duplicate rows using `df.duplicated()`.
   - No duplicate rows were found.

3. **Converted Data Types**
   - `Dt_Customer` converted from object to **datetime** format for proper date handling.
   - Other columns kept in appropriate numeric types (`int64` or `float64`).

4. **Standardized Text Columns**
   - Columns `Education` and `Marital_Status` were converted to **lowercase** and stripped of extra spaces.
   - Example: `'Graduation '` → `'graduation'`

5. **Renamed Columns**
   - Column names were converted to **lowercase** and spaces replaced with underscores for consistency.
   - Example: `'Year_Birth'` → `'year_birth'`

---

## Final Dataset
- **No missing values**  
- **No duplicate rows**  
- All columns have **correct datatypes**  
- **Cleaned dataset saved as:** `Customer_Personality_Cleaned.csv`  

---

## Tools Used
- Python 3 (Google Colab / Jupyter)
- Pandas library


---

## How to Use
1. Clone this repository.
2. Open `Task_1.ipynb` in Jupyter or Google Colab to see the data cleaning steps.
3. The cleaned dataset `Customer_Personality_Cleaned.csv` is included in this repository and is ready for analysis or visualization.

---

## Notes
- This task focuses only on **data cleaning and preprocessing**.  
- **Scaling, normalization, or label encoding** were not applied as they are not required in this step.
