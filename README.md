# Aircraft Engine Predictive Maintenance (PdM) ✈️
**Statistical Learning for Time-To-Failure (TTF) & Binary Classification**

## 📌 Project Overview
This project implements a robust Predictive Maintenance framework for aircraft engines using sensor telemetry data. [cite_start]The goal is to optimize maintenance scheduling by accurately predicting the Remaining Useful Life (RUL) and identifying engines at risk of failure within a 30-cycle window[cite: 14, 21].

## 🛠️ Tech Stack
* **Language:** Python 3.9+
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook (Anaconda)

## 📊 Methodology
### 1. Feature Engineering & EDA
* [cite_start]**Fleet-wide Correlation:** Analyzed sensor relationships to identify the physical basis for engine degradation[cite: 10, 53].
* [cite_start]**Rolling Statistics:** Implemented a 10-cycle rolling average to smooth sensor noise and capture long-term trends[cite: 48].

### 2. Regression Model (TTF Prediction)
* [cite_start]**Model:** Gradient Boosting Regressor[cite: 36, 54].
* [cite_start]**Metric:** Evaluated using Root Mean Squared Error (RMSE) against ground truth data[cite: 37, 62].

### 3. Classification Engine (Fault Detection)
* [cite_start]**Model:** Random Forest Classifier (200 Estimators)[cite: 39, 55].
* [cite_start]**Logic:** Binary classification (1 = Faulty if TTF ≤ 30 cycles; 0 = Healthy)[cite: 30].
* [cite_start]**Evaluation:** Optimized for Precision and Recall to minimize false negatives[cite: 61, 63].

## 📈 Key Results
* [cite_start]**Regression:** Achieved a competitive RMSE, effectively tracking engine health cycles[cite: 58].
* [cite_start]**Classification:** High F1-score in detecting "At-Risk" engines using the Confusion Matrix[cite: 59].

## 📂 Data Sources
[cite_start]The dataset simulates run-to-failure scenarios for 100 engines based on 4 anonymized sensor measurements[cite: 25, 26].