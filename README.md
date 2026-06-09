# Air-Quality-Indexing
## Step 1: Acquire & Understand the Dataset
https://www.kaggle.com/datasets/jocelyndumlao/classroom-indoor-air-quality-time-seriesbangladesh

## Typical features in air quality datasets include:
* Date/Time → temporal dimension.
* Pollutant concentrations (e.g., PM2.5, PM10, CO₂, NO₂).
* Environmental variables (temperature, humidity, wind speed).

Each row = a measurement at a given time.
 This dataset is multivariate, time-series, and continuous.

## Step 2: Cleaning the Data
Handle missing values: Drop or impute (e.g., mean/median for continuous variables).
Remove duplicates: Ensure no repeated timestamps.
Outlier detection: Extreme pollutant values may be sensor errors.
Feature engineering: Create rolling averages (e.g., 24-hour PM2.5 mean).

## Step 3: Exploratory Data Analysis (EDA)
Plot pollutant trends over time.
Correlation analysis between pollutants and weather variables.
Identify seasonal/temporal patterns (e.g., higher PM2.5 during dry months).

## Step 4: Dimension Reduction (Optional)
Use PCA to reduce correlated features (e.g., PM2.5 and PM10 often move together).
This simplifies clustering/classification and improves interpretability.

## Step 5: Algorithm Selection
Classification: - Our goal is to predict air quality categories (e.g., “Good”, “Moderate”, “Unhealthy”).
We will use Random Forests.
Justification:- Handles non-linear relationships and easy to interpret for policy/health recommendations.
