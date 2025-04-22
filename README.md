# Assessing the Macroeconomic Outlook of Japan with VAR-X Model

###### Contributors: Ojo Oluwafemi, Muhammad Bello, Steven Yu & Abdulwasiu Ghazali

## Overview
This project implements a multivariate time series analysis of Japan's macroeconomy using a Vector Autoregression model with exogenous macroeconomic variables (VAR-X). The study characterizes dynamic interdependencies among key Japanese macroeconomic indicators and generates out-of-sample forecasts. Japan presents a fascinating case study given its distinctive macroeconomic environment characterized by persistent deflationary pressures, unconventional monetary policy implementation, and significant exposure to external shocks as a major trading economy.

## Research Objectives/Questions
1. Analyze the dynamic relationships between Japan's key macroeconomic variables including real GDP, inflation, interest rates, exchange rates, and equity prices
2. Examine how global economic conditions (represented by exogenous variables) affect Japan's macroeconomic performance
3. Evaluate the forecasting performance of the VAR-X model compared to a Random Walk benchmark
4. Understand Japan's unique macroeconomic transmission mechanisms given its historical deflationary environment and unconventional monetary policies

## Method/Technique
- **Model**: Vector Autoregression with exogenous variables (VAR-X)
- **Variables**:
  - Endogenous: Real GDP (y), inflation (Dp), short-term interest rate (r), long-term interest rate (lr), real effective exchange rate (ep), equity prices (eq), metal prices (pmetal)
  - Exogenous: Global oil prices (poil) and country-specific foreign variables (ys, Dps, rs, lrs, eqs)
- **Data**: Quarterly data from 1979Q2 to 2022Q3.
- **Data Sources**:
  - Haver Analytics
  - IMF's International Financial Statistics Data
  - IMF's Primary Commodity Prices Monthly Data
  - Brent crude oil price from Bloomberg
  - Foreign Variables predetermined from GVAR panel

- **Analysis**:
  - Unit root tests (Augmented Dickey-Fuller)
  - VAR-X model estimation with optimal lag selection
  - Out-of-sample forecasting performance evaluation
  - Comparison with Random Walk benchmark using Root Mean Square Error (RMSE)

## Appendix
- For complete details of the analysis, methodology, results, and conclusions, please see the full report [here](resources/japan_macroeconomic_outlook_report.pdf)
- For the GVAR dataset, see [here](resources/CountryData1979Q2-2023Q3.xls)
- For the R-code used for the project, see [here](resources/japan_varx.Rmd)
