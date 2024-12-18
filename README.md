# COVID-19 Impact Analysis

This repository contains an analysis of the impacts of COVID-19 using Python. The analysis involves data preparation, aggregation, and visualization to understand the pandemic's effects on various countries.

## Table of Contents
1. [Introduction](#introduction)
2. [Data Preparation](#data-preparation)
3. [Data Aggregation](#data-aggregation)
4. [Analysis and Visualization](#analysis-and-visualization)
5. [Top 10 Countries with Highest COVID-19 Cases](#top-10-countries-with-highest-covid-19-cases)
6. [GDP Analysis](#gdp-analysis)

---

## Introduction
The goal of this project is to analyze the impacts of COVID-19 on various countries by combining datasets, aggregating data, and visualizing key metrics such as total cases, total deaths, stringency index, and GDP changes.

---

## Data Preparation
The following datasets were used:
1. **Transformed Data**: Contains metrics like Human Development Index (HDI), Stringency Index (STI), population, etc.
2. **Raw Data**: Contains metrics like total cases, total deaths, population, and GDP.

### Libraries Used
- `pandas` for data manipulation
- `plotly` for data visualization

### Steps:
1. Imported necessary libraries.
2. Loaded the datasets:
   - `transformed_data.csv`
   - `raw_data.csv`
3. Displayed initial impressions of both datasets using `.head()`.

---

## Data Aggregation
The datasets were combined to create a new aggregated dataset with the following columns:
- Country Code
- Country Name
- Human Development Index (HDI)
- Total Cases
- Total Deaths
- Stringency Index (STI)
- Population

### Aggregation Process:
1. Calculated average HDI and STI for each country.
2. Summed up total cases and deaths for each country.
3. Normalized population values.

---

## Analysis and Visualization

### Observations:
1. Unequal number of samples per country in the dataset.
2. Mode of sample counts was determined to be 294.

### Key Metrics:
- **Stringency Index**: Indicates the strictness of government measures.
- **Population**: Average population values were normalized across countries.

---

## Top 10 Countries with Highest COVID-19 Cases
The top 10 countries with the highest total cases were identified and sorted in descending order:

| Country Code | Country        | HDI    | Total Cases   | Total Deaths   | Stringency Index | Population |
|--------------|----------------|--------|---------------|----------------|------------------|------------|
| USA          | United States  | 0.924  | 746,014,098   | 26,477,574     | 3.35             | 19.62      |
| BRA          | Brazil         | 0.759  | 425,704,517   | 14,340,567     | 3.14             | 19.17      |
| IND          | India          | 0.640  | 407,771,615   | 7,247,327      | 3.61             | 21.04      |
| RUS          | Russia         | 0.816  | 132,888,951   | 2,131,571      | 3.38             | 18.80      |
| PER          | Peru           | 0.5995 | 74,882,695    | 3,020,038      | 3.43             | 17.31      |

---

## GDP Analysis
Two additional columns were added to analyze GDP changes before and during COVID-19:
1. **GDP Before COVID**
2. **GDP During COVID**

### Example Data:
| Country        | GDP Before COVID ($) | GDP During COVID ($) |
|----------------|-----------------------|-----------------------|
| United States  | 65,279.53            | 63,543.58            |
| Brazil         | 8,897.49             | 6,796.84             |
| India          | 2,100.75             | 1,900.71             |

---

## Conclusion
This analysis provides insights into how different countries were impacted by COVID-19 in terms of health metrics (cases and deaths) and economic factors (GDP). The top affected countries were identified based on their total cases and deaths.

Further visualizations can be created using Plotly to explore trends over time or correlations between metrics such as HDI and stringency index.

---

## How to Run
1. Clone this repository.
2. Install required libraries using `pip install pandas plotly`.
3. Open the Jupyter Notebook (`Covid19_Impct_analysis.ipynb`) to explore the analysis step-by-step.
