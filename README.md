# Farm Produce Data Cleaning Project

## Overview

This project focuses on cleaning and preparing a dataset containing farm produce information for proper reporting and analysis. The cleaning process was completed using Microsoft Power BI Power Query.

## Data Source

The dataset used for this project is a CSV file titled **Farm_Produce_Data.csv**.
It contains fields such as:

- Quantity Harvested
- Record_id
- Date
- Farmer_name
- Buyer
- Region
- Payment Status
- Harvest Location
- Unit_price
- Total_value

The data appears to have been collected from multiple contributors which introduced inconsistencies and missing values.

## Cleaning Steps

All cleaning was performed inside Power Query. The following transformations were carried out:

### 1. Trimmed and Cleaned Text Fields

Applied:

- **Trim** to remove extra spaces
- **Clean** to eliminate non-printable characters
  This improved consistency in text columns such as Buyer and Location.

### 2. Standardized Text Case

Converted categorical fields into a consistent format such as Proper Case or Upper Case for easier grouping and analysis.

### 3. Handled Missing Values

Different strategies were applied based on data type:

- **Quantity_Harvested (numeric)**
  Replaced missing values with the **median** to reduce the impact of outliers.
- **Buyer and Payment_Status (categorical)**
  Filled missing values with null.
  When unclear, values were left null instead of making assumptions.

### 4. Standardized Dates

Ensured all dates used the same recognizable date format for accurate sorting and filtering.

## Challenges Faced

- Mixed formats including inconsistent date entries and text casing.
- Very high missing values in some columns made replacement decisions difficult.
- Missing numeric values required careful imputation to avoid analysis errors.

## Final Output

The final cleaned dataset is:

- Free from duplicate records
- Standardized for consistency
- Ready for analysis and visualization in Power BI or other analytical tools

## Author

Data Cleaning and Documentation by [GROUP 5]
