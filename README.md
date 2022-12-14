# Snippets for Analytics
## Overview
This collection contains Python snippets for data analytics. The goal is to provide a template to quickly get a preliminary overview of a new data set.

## Data cleaning, overview and EDA
The [Cleaning and EDA](analytics_cleaning_eda.ipynb) snippet contains code to perform basic checks, type conversion, data cleaning incl. imputation and outlier treatment, and exploratory data analysis (EDA).

### Basic workflow
```mermaid
flowchart LR
subgraph 1[1. Load and Check]
    A[Load Data]--> B[Overview and Basic Checks] --> C[Type Conversion]
end
subgraph 2[2. Data Cleaning]
    C--> D[Drop NaN and Duplicates]--> E[Imputation] --> F[Treatment of Outliers]
end
subgraph 3[3. Exploratory Data Analysis - EDA]
    F--> G[Plotting univariate distributions]--> H[Plotting bivariate distributions]
end
```
