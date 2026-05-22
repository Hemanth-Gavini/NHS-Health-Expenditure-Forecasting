# NHS Health Expenditure Forecasting

MSc Data Science Dissertation Project — Coventry University (2025)

This project forecasts UK national healthcare expenditure using machine 
learning and time series analysis to support policy planning decisions.


## Project Overview

Healthcare spending is one of the largest budget items for any government.
This project builds a data-driven forecasting system that analyses 10+ years
of NHS and national health expenditure data to predict future spending 
patterns, identify cost surges, and support smarter policy decisions.

The goal was to move beyond simple trend lines and build a model that 
accounts for regional differences, seasonal effects, and demographic 
factors — giving policymakers a reliable tool for budget simulation.


## Key Results

- Forecasting accuracy of 95% on held-out test data
- Over 100,000 demographic and regional records processed
- 10+ years of historical spending data analysed
- Potential cost savings of 20% identified through preventive initiatives
- Interactive Power BI dashboard delivered for policymaker use



## Problem Statement

The NHS faces increasing budget pressure every year. Traditional forecasting 
methods treat spending as a single national figure, which misses the regional 
and demographic variation that drives actual costs.

This project addresses four core problems:

- NHS budgets are under increasing pressure with limited forecasting tools
- Traditional methods lack regional granularity
- Policymakers need interactive tools to simulate future budget scenarios
- Inefficient allocations lead to preventable cost overruns



## Technologies Used

- Python — main language for data cleaning, EDA, and modelling
- SQL — data extraction and transformation
- Power BI — interactive dashboard development
- ARIMA and SARIMAX — time series forecasting models
- Prophet — advanced seasonal forecasting by Meta
- Pandas and NumPy — data manipulation and analysis
- Matplotlib and Seaborn — data visualisation
- Scikit-learn — machine learning model building and evaluation



## Methodology

### Step 1 — Data Collection and Cleaning

I sourced over 10 years of national healthcare spending data from 
publicly available datasets. The raw data contained over 100,000 records 
across demographic groups and regions. Cleaning involved handling missing 
values through interpolation, removing outliers, and standardising formats 
across different regional datasets.

### Step 2 — Exploratory Data Analysis

Before modelling, I analysed spending trends by region including Asia, 
Middle East, and Europe. I identified seasonal patterns and cost surge 
periods by visualising historical Current Health Expenditure as a 
percentage of GDP by region from 2000 to 2021. This stage shaped 
which features were included in the final models.

### Step 3 — Forecasting Models

I tested four forecasting approaches and selected the best per region 
based on RMSE scores:

- ARIMA was used as the baseline time series model
- SARIMAX added seasonal adjustment with external demographic variables
- Prophet handled holiday effects and complex seasonality patterns
- Linear Regression served as a fallback for regions with sparse data

### Step 4 — Power BI Dashboard

The final deliverable was an interactive dashboard built in Power BI. 
It includes regional slicers, year filters, KPI cards comparing forecast 
versus actual spend, and a budget simulation tool that allows policymakers 
to model different future spending scenarios up to 2035.


## Key Findings

Regional disparities in healthcare spending were identified across 
demographic groups, with certain regions showing consistently 
inefficient allocation patterns.

Cost surge periods were detected and flagged in the data, allowing 
targeted intervention planning.

The analysis showed that preventive health initiatives could reduce 
national healthcare costs by approximately 20% over a five year period.

The 95% forecasting accuracy was achieved on held-out test data using 
a combination of SARIMAX and Prophet models depending on the region.
