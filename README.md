# Monthly Gold Price Prediction Analysis (1833 - 2026)

## Project Overview
This repository contains a machine learning implementation designed to forecast monthly gold prices. The project utilizes a time-series forecasting approach, transforming historical price data into a supervised learning problem through the application of lag features. The model is trained on global gold price records spanning from 1833 to early 2026.

## Technical Specifications
* **Operating System:** Fedora 43 Workstation
* **Development Environment:** Dell Latitude E5540
* **Programming Language:** Python 3.x
* **Core Libraries:** Pandas, Scikit-Learn, NumPy

## Implementation Logic
The project follows a systematic data science workflow:
1. **Data Preprocessing:** Handled datetime objects and managed missing values (NaN) resulting from feature shifting.
2. **Feature Engineering:** Implemented a univariate time-series strategy by creating a "Previous_Month" lag feature (T-1) to predict the current month (T).
3. **Model Training:** Employed the Linear Regression algorithm to model the relationship between consecutive monthly price points.
4. **Validation Strategy:** Data was partitioned into an 80/20 train-test split to validate the model's predictive capabilities on unseen data.

## Performance Evaluation
The model's performance was measured using standard regression metrics. Given the high valuation of gold per troy ounce, the results indicate a high degree of precision for short-term forecasting.

| Evaluation Metric | Statistical Value |
| :--- | :--- |
| **Mean Absolute Error (MAE)** | **6.63** |
| **Mean Squared Error (MSE)** | 286.64 |
| **Root Mean Squared Error (RMSE)** | 16.93 |

### Interpretation
The Mean Absolute Error (MAE) of 6.63 signifies that, on average, the model's predictions deviate by only $6.63 from the actual market price. Considering current market prices exceed $5,000 per ounce, this represents a highly optimized fit for trend-following scenarios.

## Installation and Usage
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YourUsername/Gold-Price-Prediction-ML.git
   ```
2. **Install Required Packages:**
   ```bash
   pip install pandas scikit-learn
   ```
3. **Execute the Script:**
   ```bash
   python Gold_Price_Model.py
   ```

## Author
**Arsalan Jamal**
Machine Learning and Artificial Intelligence Developer

---
