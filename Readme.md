# Waze User Churn Dataframe Analysis

## Project Overview

This project, part of Google's "Get Started in Python" course, focuses on analyzing Waze user churn data to understand and prevent user drop-off. We employ Python for data analysis.

## Python Concepts Utilized

- **Data Loading**: We used Pandas to load the dataset.
- **Data Inspection**: We examined data structure with `df.head(10)` and `df.info()`.

## Data Cleaning

- **Handling Missing Data**: To address missing data, we used Pandas' `.isnull()` and `.notnull()` methods to create separate dataframes for rows with missing 'label' values (`null_df`) and rows without missing values (`not_null_df`). This allowed us to isolate and investigate instances of user churn.
- **Descriptive Statistics**: We calculated summary statistics, including means and medians, to gain insights into the distribution of key variables. The `describe()` method provided an overview of the dataset's central tendencies.

## Data Analysis

- **Missing Value Analysis**: To analyze missing values, we used Pandas' `.isnull()` method to identify rows with missing 'label' values and examined these instances. This step helped us understand the extent of missing data and whether any patterns existed.
- **Median Analysis**: For user behavior insights, we calculated median statistics for specific columns using the `.groupby()` method in Pandas. By grouping data by the 'label' column, we obtained median values for 'driven_km_drives', 'drives', and 'driving_days'. This allowed us to compare the behavior of users who churned with those who were retained.
- **Device Analysis**: To explore user distribution by device type, we used the `.value_counts()` method in Pandas on the 'device' column. This analysis revealed that approximately 64% of users were iPhone users, while 36% were Android users.
- **Churn Rate Comparison**: To compare churn rates, we examined the proportion of users who churned for both iPhone and Android users. We found similar churn rates for both device types, differing by only one percentage point.

These data cleaning and analysis steps, coupled with Python concepts, are fundamental in unraveling user churn patterns and form the basis for optimizing user retention strategies and data-driven decisions for Waze's growth.



