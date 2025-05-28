# Weather Prediction Model

This project builds a machine learning model to predict future weather conditions of **Oakland** using historical weather data collected by **Oakland International Airport.**

## Overview

We aim to forecast **maximum temperatures** using a dataset from [NOAA's Climate Data Online](https://www.ncdc.noaa.gov/cdo-web/search). The data originates from a weather station located at **Oakland International Airport**, which has been recording reliable weather metrics since **1948**, which is ideal for long-term pattern analysis. But for our purposes, we've only extracted data going as far back as **1960**.

### Models Used
- **Ridge Regression** (Linear model)
- **LightGBM** (Gradient boosting decision trees)

Both models are evaluated using the **Mean Absolute Error (MAE)** as the performance metric.

---

## Dataset

- Sourced from NOAA’s public climate records.
- Contains daily weather measurements.
- Covers multiple decades of data.
- The version used in this notebook was downloaded on **May 28, 2025**.

---

## Features Used

Features include:
- `max_temp`, `min_temp`
- `precipitation`
- Further features were engineered

---

## Results
- Models were evaluated using **year-by-year backtesting** to provide a robust error estimate.
- **Best MAE** was achieved with **LightGBM** using engineered features and tuned hyperparameters.

## Libraries Required

Make sure to install the following Python libraries before running the notebook:

```bash
pip install pandas numpy lightgbm scikit-learn
