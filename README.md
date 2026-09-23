# Credit Union Loan Forecasting Project

## Overview

This project was developed during my Data Analyst internship at **TruStage** to forecast eligible loan volumes at the credit union level using publicly available **NCUA data**.

The project combined data extraction and preparation using **Snowflake and SQL**, predictive modeling in **Python**, and results visualization in **Power BI**. The goal was to create accurate forecasts that could support business planning and provide insight into expected loan activity across hundreds of credit unions.

---

## Project Objectives

* Pull and combine data from multiple Snowflake data sources using SQL
* Clean, validate, and prepare historical NCUA data for modeling
* Engineer time-based features to improve forecasting performance
* Compare machine learning forecasting approaches
* Evaluate model performance on unseen data
* Visualize forecast results and model performance in Power BI
* Present findings and business insights to stakeholders

---

## Tools & Technologies

* Python
* pandas
* NumPy
* scikit-learn
* XGBoost
* Random Forest
* Snowflake
* SQL
* Power BI
* DAX
* Power Query

---

## Data Source

The project used publicly available credit union data from the **National Credit Union Administration (NCUA)**.

The data was accessed and prepared through Snowflake, where SQL was used to:

* Join information from multiple data sources
* Filter data to relevant credit unions and time periods
* Select variables used for forecasting
* Validate and inspect source data
* Prepare modeling datasets for use in Python

---

## Feature Engineering

To capture historical patterns in loan activity, I created features including:

* Lagged loan-volume variables
* Rolling averages
* Historical credit union performance
* Credit union-level characteristics
* Time-based predictors

Credit unions were also segmented based on characteristics such as size and historical volatility to evaluate model behavior across different groups.

---

## Modeling

Two primary machine learning models were evaluated:

### Random Forest

A Random Forest regression model was used to capture nonlinear relationships between historical features and future loan volumes.

### XGBoost

An XGBoost regression model was also developed using engineered lag and rolling features.

Models were trained primarily using historical data from **2024 through 2025**, with the **first six months of 2026** used as an out-of-sample testing period.

---

## Model Performance

The forecasting approach achieved approximately:

* **R²: 0.92**
* **Median MAPE: 15%**

These results indicated strong predictive performance across hundreds of credit unions.

Model performance was evaluated both overall and across different credit union segments.

---

## Power BI Visualization

Forecast outputs were loaded into **Power BI** to create business-facing visualizations of model results.

The report included views of:

* Actual vs. predicted loan volumes
* Forecast accuracy
* Credit union-level performance
* Segment-level performance
* Historical and forecast trends

The Power BI report was also used to present results and key findings to stakeholders.

---

## Project Workflow

```text
NCUA Data
    ↓
Snowflake
    ↓
SQL Data Preparation
    ↓
Python / pandas
    ↓
Feature Engineering
    ↓
Random Forest & XGBoost
    ↓
Model Evaluation
    ↓
Forecast Results
    ↓
Power BI
    ↓
Stakeholder Presentation
```

---

## Key Skills Demonstrated

* Working with public financial and credit union data
* Querying and combining data using SQL
* Working with Snowflake data sources
* Data cleaning and validation
* Feature engineering for forecasting
* Random Forest and XGBoost regression
* Forecast evaluation using R² and MAPE
* Power BI dashboard development
* Communicating analytical findings to business stakeholders
