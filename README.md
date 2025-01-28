# Arvida Predict
Arvida Predict &amp; Scenario Planning 
This repository implements a comprehensive Media Mix Modeling (MMM) analysis using Google's Lightweight MMM library for Arvida. The project aims to evaluate marketing channel effectiveness, determine return on investment (ROI), optimize budget allocation, and forecast future marketing outcomes.

### Features
Data Integration: Combines internal and external datasets, including competitor data, seasonality indices, and economic indicators.
Data Preparation: Handles data cleaning, variable transformation, and feature engineering.
Bayesian MMM: Uses Google's Lightweight MMM for advanced Bayesian modeling with carryover and adstock effects.
Media ROI Calculation: Computes contributions, ROI, and decay rates for each marketing channel.
Budget Optimization: Provides recommendations for optimal budget allocation to maximize ROI or achieve specific targets.
Scenario Planning: Enables annual and monthly forecast simulations under different marketing scenarios.
Interactive Visualizations: Generates plots for contributions, ROI, response curves, and optimized budget comparisons.

### Required Libraries
Install the dependencies using the following commands:

### Install Google's Lightweight MMM
pip install --upgrade git+https://github.com/google/lightweight_mmm.git

### Install specific dependencies
pip install matplotlib==3.6.1
pip install pandas openpyxl xlrd jax[cpu] numpyro plotly.express google-cloud-storage

### Workflow
Data Loading and Cleaning: Loads external datasets from Google Cloud Storage and preprocesses them for modeling.
Feature Engineering: Creates control variables like seasonality indices, competitor share of spend, and economic indicators.
Data Quality Checks: Handles missing values, outliers, and multicollinearity among variables.
Model Fitting: Fits a Bayesian Media Mix Model with carryover effects to estimate channel contributions.
Optimization: Optimizes budget allocation across marketing channels to maximize KPIs.
Scenario Analysis: Performs scenario planning for annual or monthly forecasts.
Visualization: Generates intuitive plots for media contributions, ROI, and response curves.

### Key Results
  1. Media Contributions
  Plots the percentage contribution of each channel to the target KPI (total leads).
  
  2. Return on Investment (ROI)
  Calculates the ROI for each channel, helping assess cost-effectiveness.
  
  3. Optimization Results
  Visualizes budget allocation before and after optimization, comparing the predicted performance.
  
  4. Response Curves
  Shows how the target KPI responds to incremental media spending, highlighting diminishing returns.
