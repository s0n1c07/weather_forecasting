# Air Quality & Traffic Data Analysis

A Python‑based pipeline to explore, model and predict urban PM2.5 concentrations by integrating meteorological, pollutant and TomTom traffic data for Delhi.

## 🔍 Project Overview

- **Goal**: Understand drivers of fine‑particle pollution (PM2.5) and build accurate predictive models.  
- **Approach**:  
  1. **Data ingestion** from CPCB stations (Jan–Jul 2024) and TomTom traffic APIs  
  2. **Cleaning & Imputation** to handle missing sensor readings  
  3. **Feature Engineering** to derive traffic‑pollution interaction metrics  
  4. **Modeling** with linear regression, Random Forest, XGBoost, LightGBM, ElasticNet  
  5. **Evaluation** using RMSE, MAE, R²

## 📈 Key Highlights
Imputation: time‑based interpolation, group‑median fills, forward/backward filling

Transformations: Yeo–Johnson for skewed pollutant/traffic data; Min–Max scaling

## New Features:

Congestion Factor (1 – current_speed / free_flow_speed)

PM2.5/PM10 Ratio, Humidity × WindDir, Traffic Index

Best Model: Gradient‑boosting (XGBoost/LightGBM) achieved lowest RMSE (~2–3 µg/m³)

## Insights:

High congestion & low wind speeds drive PM2.5 spikes

Regional variations: north‑west Delhi stations showed consistently higher pollution

## 📄 Reports & Further Reading
Detailed methodology, full statistical tables and plots: see reports/its.docx

