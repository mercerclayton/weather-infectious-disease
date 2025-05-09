# Weather Variables and Infectious Disease Incidence (2015–2024)

Predicting infectious disease outbreaks in Hong Kong using weather data.

## Table of Contents

* [Project Description](#project-description)
* [Data](#data)
* [Environment Setup](#environment-setup)
* [Methods](#methods)

## Project Description

This project analyzes the relationship between monthly weather variables (rainfall, humidity, mean temperature) and infectious-disease case counts in Hong Kong from 2015 to 2024. By applying statistical tests and machine learning models, it generates actionable insights for public-health forecasting and resource allocation.

## Data

* `data/2015-2024 Disease.xlsx`: Monthly disease case counts.
* `data/CLMMAXT_HKO_.csv`: Daily maximum temperature from Hong Kong Observatory.
* `data/CLMMINT_HKO_.csv`: Daily minimum temperature from Hong Kong Observatory.
* `data/CLMTEMP_HKO_.csv`: Daily mean temperature from Hong Kong Observatory.
* `data/daily_HKO_RF_ALL.csv`: Daily rainfall from Hong Kong Observatory.
* `data/daily_HKO_RH_ALL.csv`: Daily relative humidity from Hong Kong Observatory.
* `processed_disease_weather_data.xlsx`: Combined and preprocessed monthly weather and disease data.

## Environment Setup

1. Clone the repository:

   ```bash
   git clone <repo_url>
   cd <repo_folder>
   ```
2. Create a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels pydotplus ipython
   ```

## Methods

* **Statistical Tests**: Two-sample t-tests to assess significance of weather variables on outbreak incidence.
* **Logistic Regression**: Quantify how each weather factor affects outbreak probability.
* **Decision Tree**: Identify threshold conditions for high-risk weather profiles.
