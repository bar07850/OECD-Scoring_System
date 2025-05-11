# OECD Real Estate Investment Scoring System

This project develops a data-driven scoring system to evaluate the investment attractiveness and risk of real estate markets across OECD countries.  
It integrates macroeconomic, political, and demographic indicators into structured scoring models to help identify ideal real estate investment locations.

## 📋 Project Overview

The project has three core stages:
1. **Data Cleaning** → Prepare clean datasets for analysis.
2. **Investment Stability Scoring** → Develop an investment scoring model.
3. **Risk Evaluation Model** → Build an alternative model to evaluate market risk.

This portfolio project demonstrates a full data science pipeline:
- Data wrangling and cleaning
- Feature engineering
- Predictive modeling
- Risk assessment
- Data visualization

## 📦 Datasets Used

| Dataset | Description |
|--------|-------------|
| Labor Force | Total labor force per country |
| Unemployment Rate | Unemployment data by country/year |
| Corruption Index | Country-level corruption perceptions |
| Public Sector Debt | Government debt levels |
| Foreign Direct Investment | FDI inflows |
| GDP | National GDP in USD |
| Political Stability | Governance and political risk indicators |
| Population Growth | Demographic trends |
| Birth Rate | Birth rates by country |

*All datasets were cleaned to focus on the 38 OECD countries.*

---

## 🛠️ Methodology

### 📄 1. CleanData.ipynb
- Filters raw datasets for OECD countries
- Handles missing values
- Selects years 2010–2023
- Outputs clean CSV files

### 📊 2. OECD_ScoringModel.ipynb
- Merges all cleaned macro datasets
- Imputes missing values using median
- Scales numerical features using StandardScaler
- Computes a custom **Investment Stability Index**:

### 📊 3. CL_IRRS.ipynb (Risk Assessment Model)
- Loads cleaned macroeconomic datasets
- Reshapes all data into a consolidated long format
- Merges indicators to create a master Risk Dataset
- Normalizes data using MinMaxScaler
- Provides a flexible dataset for building a Risk Scoring Model
- Prepares the data for further statistical analysis, ranking, or machine learning risk evaluation
- Includes country-level checks for missing risk data
