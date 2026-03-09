# Aircraft Engine Predictive Maintenance (PdM) ✈️
**Statistical Learning for Time-To-Failure (TTF) & Binary Classification**

## 📌 Project Overview
This project implements a robust Predictive Maintenance framework for aircraft engines using sensor telemetry data. The goal is to optimize maintenance scheduling by accurately predicting the Remaining Useful Life (RUL) and identifying engines at risk of failure within a 30-cycle window.

## 🛠️ Tech Stack
* **Language:** Python 3.9+
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook (Anaconda)

## 📊 Methodology
### 1. Feature Engineering & EDA
* **Fleet-wide Correlation:** Analyzed sensor relationships to identify the physical basis for engine degradation.
* **Rolling Statistics:** Implemented a 10-cycle rolling average to smooth sensor noise and capture long-term trends.

### 2. Regression Model (TTF Prediction)
* **Model:** Gradient Boosting Regressor.
* **Metric:** Evaluated using Root Mean Squared Error (RMSE) against ground truth data.

### 3. Classification Engine (Fault Detection)
* **Model:** Random Forest Classifier (200 Estimators).
* **Logic:** Binary classification (1 = Faulty if TTF ≤ 30 cycles; 0 = Healthy).
* **Evaluation:** Optimized for Precision and Recall to minimize false negatives.

## 📈 Key Results
* **Regression:** Achieved a competitive RMSE, effectively tracking engine health cycles.
* **Classification:** High F1-score in detecting "At-Risk" engines using the Confusion Matrix.

## 📂 Data Sources
The dataset simulates run-to-failure scenarios for 100 engines based on 4 anonymized sensor measurements.
