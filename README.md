# smart-campus-intelligence


A smart dashboard to monitor and predict campus resource usage — including **electricity consumption**, **mess footfall**, **WiFi usage**, and **student attendance** — built with Python, Machine Learning, and Streamlit.

---
##  What is this project?

Campus resources like **electricity, WiFi, mess food, and student attendance** are managed manually in most colleges — leading to wastage, poor planning, and inefficiency.

This project builds a **smart monitoring and prediction system** that:
-  Analyzes historical usage patterns
-  Predicts future resource demand using Machine Learning
-  Detects anomalies and unusual spikes automatically
-  Displays everything on a live, interactive Streamlit dashboard


---

---

##  Problem Statement

| Problem | Impact |
|---|---|
| Mess food prepared for 500 students but only 300 show up on weekends | Food wastage |
| WiFi overloads every evening with no prior warning | Poor user experience |
| Electricity consumed blindly with no peak detection | High energy cost |
| Attendance tracked manually with no pattern analysis | Administrative overhead |

**Our solution:** A unified dashboard that predicts all four resources in advance using ML models trained on time-series data.

---



---

##  Features

-  **Electricity Monitoring** — Daily usage trends, hourly patterns, RF + ARIMA forecasting
-  **Mess Footfall Prediction** — Lunch/dinner peak detection, weekday vs weekend analysis, anomaly flagging
-  **WiFi Usage Forecasting** — Evening peak prediction, spike detection
-  **Attendance Analytics** — 500-student simulation, weekday vs weekend attendance comparison
-  **Anomaly Detection** — Automatic flagging of unusual mess footfall using statistical thresholds
-  **Interactive Dashboard** — All insights in one place, built with Streamlit

---


---
# smart-campus-intelligence

> **Predict. Monitor. Optimize.** — A smart ML-powered dashboard for managing campus resources efficiently.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red?style=flat&logo=streamlit)
![ML](https://img.shields.io/badge/Machine%20Learning-RandomForest%20%7C%20ARIMA-green?style=flat)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat)







---

## Machine Learning Models

| Resource | Model | Features Used | Metric | Result |
|---|---|---|---|---|
| Mess Footfall | Random Forest Regressor | hour, day of week | MAE + R² | ✅ Low error |
| WiFi Usage | Random Forest Regressor | hour, day of week, mess footfall | MAE + R² | ✅ Low error |
| Electricity | Random Forest + ARIMA | hour, day of week / time-series | MAE | ✅ Compared both |
| Attendance | Random Forest Classifier | day of week, student id | Accuracy | ✅ ~80%+ |

### Why Random Forest?
- Handles non-linear patterns well
- Works great with time-based features like hour and day
- Robust to noise in synthetic/real data
- No need for feature scaling

### Why ARIMA for Electricity?
- Electricity consumption is a classic time-series problem
- ARIMA captures trends and seasonality in sequential data
- Used to compare against Random Forest performance

---

### Dashboard : http://10.81.55.138:8501


