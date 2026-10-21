
# Refugee Dynamics in Europe

### Political, Socio-Economic and Demographic Analysis

[View Project Portfolio](https://lorenzobettin.github.io/projects/refugee-dynamics/)

## Overview

This project investigates relationships between refugee
populations, political orientation and socio-economic
characteristics across European countries and selected
international comparators.

Using Python and statistical modelling, the analysis
combines refugee population statistics with historical
political and economic indicators.

The aim is to explore patterns in refugee populations and
assess whether selected explanatory variables are
statistically associated with these differences.

## Research Question

How are political, socio-economic and demographic factors
associated with refugee populations across European
countries?

## Dataset

The cleaned analysis includes:

- 36 countries, including non-European comparators
- 1,635 country-year observations
- Historical refugee population data
- Political, economic and demographic indicators

### Data Sources

- World Bank: Refugee population statistics
  https://data.worldbank.org/indicator/SM.POP.REFG

- Comparative Political Data Set (CPDS)
  https://cpds-data.org/

## Methodology

### 1. Data Collection and Integration

Combined historical refugee population data with
political and socio-economic variables from the CPDS.

### 2. Data Preprocessing

- Reshaped country-year datasets
- Merged observations from different sources
- Addressed missing values
- Encoded categorical political variables
- Calculated refugee-to-population ratios

### 3. Exploratory Data Analysis

Examined:
- Refugee population trends over time
- Differences across countries
- Refugee-to-population ratios
- Government orientation and population size

### 4. Statistical Modelling

Applied ordinary least squares (OLS) regression to
investigate associations between absolute refugee
population counts and selected explanatory variables.

The model was evaluated using:
- Train-test splitting
- R-squared
- Mean squared error
- Five-fold cross-validation

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- scikit-learn
- statsmodels
- Jupyter Notebook

## Key Findings

### Government Orientation

Government-orientation indicators showed limited
statistical significance in the reported regression
specification.

This does not imply that government policy has no
influence on refugee outcomes.

### Socio-Economic Indicators

Several economic and labour-market indicators showed
statistical associations with refugee population counts.

These relationships should not be interpreted as causal.

### Model Evaluation

The original notebook reported:

- Test R²: approximately 0.696
- Mean five-fold cross-validation R²: approximately -10.02

The strongly negative cross-validation performance
suggests poor generalization and substantial model
instability.

Accordingly, the regression is presented as exploratory
rather than a reliable predictive model.

## Limitations

The analysis has several limitations:

- Correlation does not establish causation.
- Refugee dynamics are influenced by factors not fully
  represented in the dataset.
- Model performance varies substantially across folds.
- Country-level aggregation can conceal important
  within-country differences.

## Source Code

The original analysis is provided in:

`EU_refugees.ipynb`

The notebook contains the data-processing workflow,
visualizations, regression modelling and evaluation.

## Reproducibility

The notebook references external World Bank and CPDS
datasets. Required input files are not included in this
repository unless separately uploaded.

Some original local file paths may need to be adjusted
before execution in a different environment.

## Portfolio

[View the complete project case study](https://lorenzobettin.github.io/projects/refugee-dynamics/)
