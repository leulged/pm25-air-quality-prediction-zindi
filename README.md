# 🌍 Urban Air Pollution Prediction

This repository contains a solution to the **Zindi Urban Air Pollution Challenge**, which aims to predict air quality (PM2.5 concentration) in cities around the world using satellite and environmental data.

## 🚀 Problem Statement

> Can you predict air quality in cities around the world using satellite data?

Air pollution is a major global issue that affects millions of lives each year. This project utilizes data from the **World Air Quality Index Project** to build a machine learning model capable of accurately predicting air pollution levels across various cities and countries.

## 📂 Dataset

- **Train.csv** and **Test.csv** provided by the competition.
- Features include satellite-based environmental variables, meteorological data, and location identifiers.
- Target: **PM2.5 concentration** (measured in µg/m³)

Source: [aqicn.org](https://aqicn.org) and [waqi.info](https://waqi.info)

## 🛠️ Features of This Project

✅ Duplicate Column Detection and Removal  
✅ KNN Imputation for Missing Values  
✅ LightGBM, XGBoost, and CatBoost Base Models  
✅ Hyperparameter Tuning using Optuna  
✅ Stacked Ensemble with Ridge Regressor  
✅ 5-Fold Cross-Validation for Robustness  
✅ Final Submission Generator  

## 🧠 Model Architecture

The solution uses a **stacked ensemble** approach combining the strengths of:
- LightGBM
- XGBoost
- CatBoost  
With a Ridge Regressor as the meta-learner.

This ensemble has shown strong generalization ability across diverse data distributions from different countries and time zones.

## 📈 Evaluation Metric

- **Root Mean Squared Error (RMSE)** on the validation set
- Final submission is evaluated on unseen test data by Zindi


