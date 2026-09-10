# Seasonal Agriculture Performance Analysis

**Author:** Pushkar Gaur
**Program:** VOIS AICTE Batch 2026–2027 — Major Project (Data Analytics)
**Domain:** Agriculture

## Project Overview

This project analyzes a seasonal agriculture dataset (4,000 farm records across 3 cropping seasons — Kharif, Rabi and Zaid) to uncover patterns, trends, and relationships in agricultural performance, resource usage, and economic outcomes across seasons.

> This is a pure Data Analytics project — no Machine Learning or dashboarding is included.

## Objectives

- Understand the structure and quality of the agricultural dataset
- Clean and prepare the data for analysis
- Explore seasonal patterns in the dataset
- Perform descriptive and statistical analysis
- Investigate relationships among relevant variables
- Compare agricultural performance across seasons and other meaningful groups
- Apply univariate, bivariate and multivariate visualizations
- Identify significant, evidence-based findings

## Repository Structure

```
├── Seasonal_Agriculture_Performance_Analysis_PushkarGaur.ipynb   # Main analysis notebook
├── seasonal_agriculture_performance_dataset.csv                  # Dataset used
├── Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf   # Original project brief
└── README.md
```

## Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy (statistical testing)

## Dataset

The dataset (`seasonal_agriculture_performance_dataset.csv`) contains 4,000 records with 28 columns covering:
- **Location & crop:** State, District, Crop, Season
- **Environmental conditions:** Rainfall, Temperature, Humidity, Sunlight, Soil pH/Moisture
- **Farming practices:** Irrigation Method, Fertilizer, Pesticide, Seed Quality
- **Output:** Yield, Production
- **Economics:** Market Price, Cost, Revenue, Profit
- **Resource usage:** Water Used, Water Efficiency, Disease/Pest Risk

## Approach

1. **Data Understanding** — `.head()`, `.tail()`, `.info()`, `.describe()`
2. **Data Cleaning** — missing-value imputation (season-wise median), duplicate check, outlier review (IQR method)
3. **Univariate Analysis** — season, crop, state, yield, profit, irrigation-method distributions
4. **Bivariate Analysis** — yield/profit/rainfall/water use vs. season, crop-season crosstab, correlation heatmap
5. **Multivariate Analysis** — yield by crop & season, profit by irrigation & season, fertilizer-yield relationship by season
6. **Statistical Testing** — one-way ANOVA on yield and profit across seasons
7. **Key Findings & Recommendations** — evidence-based conclusions and practical recommendations

## Key Findings (Summary)

- Profit differs **statistically significantly** across seasons (ANOVA, p < 0.05); average yield does **not** differ significantly (p ≈ 0.21) — season shapes the economics of farming more than raw output per hectare.
- Kharif season has the highest rainfall dependence and water usage, consistent with the monsoon.
- Certain crops are concentrated in specific seasons, reflecting real cropping calendars.
- Irrigation method and crop choice influence profitability as much as, or more than, season alone.

See the notebook for the full analysis, charts, and detailed conclusions.

## How to Run

1. Clone this repository
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scipy jupyter`
3. Open `Seasonal_Agriculture_Performance_Analysis_PushkarGaur.ipynb` in Jupyter Notebook / JupyterLab / Google Colab
4. Run all cells

---
*Submitted as part of the VOIS AICTE Major Project — Seasonal Agriculture Performance Analysis.*
