# Chicago Crime Arrest Prediction

Built a predictive pipeline to forecast arrest outcomes in Chicago using 7.6M+ crime records with PySpark & Power BI.

## Overview
This project uses PySpark and Spark MLlib to model arrest likelihood based on time, crime type, and location. A class imbalance challenge was tackled with model-based weighting.

## Dataset
- 7.6M+ crime records from 2001–present
- Fields: `primary_type`, `location`, `arrest`, `district`, `hour`, `date`, etc.

## Features Engineered
- Time of day & day of week
- Geospatial info (districts, wards)
- Encoded crime categories

## Model Pipeline
- Data cleaning with PySpark
- Feature engineering
- Train/validation/test split (stratified)
- Models: Logistic Regression, Random Forest, GBT
- GBT selected as best model

## Results
- Accuracy: **87.7%**
- F1 Score: **0.86**
- ROC-AUC: High 

## Power BI Dashboard
Includes:
- Arrest probability heatmap by district
- Time trends in arrest activity
- Model evaluation visuals

## Tools & Libraries
`PySpark`, `Apache Spark MLlib`, `Power BI`, `Google Colab`, `pandas`, `matplotlib`
