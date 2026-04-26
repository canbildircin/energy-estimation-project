# Energy Consumption Forecasting with XGBoost

This project focuses on predicting hourly energy consumption using time-series data from PJM Interconnection. I implemented a machine learning pipeline to analyze and forecast energy demand.

## Project Overview
The goal is to predict the energy consumption (in MW) based on historical data. I used **XGBoost Regressor**, one of the most powerful algorithms for structured data, to capture seasonal and hourly patterns.

## Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, XGBoost, Matplotlib, Seaborn, Scikit-learn
- **Tools:** Jupyter Notebook, VS Code

## Key Features
- **Time-Series Split:** Used chronological splitting (before/after 2015) to prevent data leakage.
- **Feature Engineering:** Extracted `hour`, `dayofweek`, `month`, and `quarter` from timestamps.
- **XGBoost Implementation:** Optimized with `early_stopping_rounds` to prevent overfitting.
- **Visualization:** Comparative analysis of actual vs. predicted values.

## Results
The model successfully captures the daily and seasonal fluctuations. The **Mean Absolute Error (MAE)** achieved is approximately 2902.29W.

## How to Run
1. Clone the repository: `git clone <your-repo-link>`
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebooks/analyse.ipynb` and run all cells.