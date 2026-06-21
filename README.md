[![Sales Forecasting](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=28&duration=3000&pause=1000&color=00E5FF&center=true&vCenter=true&multiline=true&repeat=true&width=600&height=100&lines=Sales+Forecasting;Time+Series+%2B+Machine+Learning;End-to-End+ML+Project+2026)](https://git.io/typing-svg)  
[![Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/) [![Scikit--Learn-1.3%2B-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white](https://img.shields.io/badge/Scikit--Learn-1.3%2B-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/) [![Statsmodels-0.13%2B-013243?style=for-the-badge&logo=python&logoColor=white](https://img.shields.io/badge/Statsmodels-0.13%2B-013243?style=for-the-badge&logo=python&logoColor=white)](https://www.statsmodels.org/) [![Pandas-2.0%2B-150458?style=for-the-badge&logo=pandas&logoColor=white](https://img.shields.io/badge/Pandas-2.0%2B-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/) [![NumPy-1.24%2B-013243?style=for-the-badge&logo=numpy&logoColor=white](https://img.shields.io/badge/NumPy-1.24%2B-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/) [![Matplotlib-3.7%2B-FF6F00?style=for-the-badge&logo=plotly&logoColor=white](https://img.shields.io/badge/Matplotlib-3.7%2B-FF6F00?style=for-the-badge&logo=plotly&logoColor=white)](https://matplotlib.org/)  
[![GitHub stars](https://img.shields.io/github/stars/basitali08/sales-forecasting?style=social)](https://github.com/basitali08/sales-forecasting) [![GitHub forks](https://img.shields.io/github/forks/basitali08/sales-forecasting?style=social)](https://github.com/basitali08/sales-forecasting)

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Pipeline](#project-pipeline)
- [Model Performance](#model-performance)
- [Key Findings](#key-findings)
- [Visualizations](#visualizations)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [Author](#author)

---

## 🔍 Overview

> **Forecast future sales with 89% accuracy using Time Series Analysis & Machine Learning — enabling data-driven business planning.**

Accurate sales forecasting is critical for inventory management, staffing, and budgeting. This project builds a complete forecasting system that:

- Analyzes **730 days (2 years)** of historical sales data
- Detects **seasonal patterns** (weekly, monthly, yearly)
- Compares **Linear Regression & Random Forest Regressor**
- Achieves **0.89 R² Score** with the best model
- Generates **30-day future sales predictions**

[![R2-Score](https://img.shields.io/badge/R2--Score-0.89-success?style=flat-square&labelColor=1a1a2e&color=00e676)](https://github.com/basitali08/sales-forecasting)
[![MAE](https://img.shields.io/badge/MAE-850-success?style=flat-square&labelColor=1a1a2e&color=00e676)](https://github.com/basitali08/sales-forecasting)
[![RMSE](https://img.shields.io/badge/RMSE-1150-success?style=flat-square&labelColor=1a1a2e&color=00e676)](https://github.com/basitali08/sales-forecasting)
[![MAPE](https://img.shields.io/badge/MAPE-8.2%25-success?style=flat-square&labelColor=1a1a2e&color=00e676)](https://github.com/basitali08/sales-forecasting)
[![Dataset](https://img.shields.io/badge/Dataset-730_days-blue?style=flat-square&labelColor=1a1a2e&color=0066ff)](https://github.com/basitali08/sales-forecasting)

---

## 📊 Dataset

**Source:** Retail Sales Dataset (Kaggle)

| Feature | Type | Description |
|---------|------|-------------|
| `date` | DateTime | Transaction date |
| `sales` | Numeric | Daily revenue amount |
| `product_category` | Categorical | Electronics, Clothing, Home, Food |
| `promotion` | Binary | 0 = No promotion, 1 = Promotion active |
| `is_holiday` | Binary | 0 = Regular day, 1 = Holiday |

> **Pattern:** Strong weekly seasonality with upward trend over 2 years.

---

## 🔄 Project Pipeline

```
📥 Load Data → 🔍 EDA Viz → 📈 Decompose Trend → 🔧 Feature Eng → 🤖 Train Models → 📊 Evaluate → 🔮 Forecast Future
```

**Step-by-step:**

1. **Data Loading** — Load CSV with 730 days of sales data
2. **EDA** — Visualize trends, seasonality, distributions
3. **Time Decomposition** — Separate trend, seasonal, residual components
4. **Stationarity Test** — Augmented Dickey-Fuller test
5. **Feature Engineering** — Create lag features, rolling statistics, time features
6. **Model Training** — Train Linear Regression, Random Forest
7. **Future Prediction** — Generate 30-day sales forecast

---

## 📈 Model Performance

| Model | MAE | RMSE | MAPE | R² Score |
|-------|-----|------|------|----------|
| Linear Regression | $980 | $1,320 | 9.8% | 0.85 |
| **Random Forest** | **$850** | **$1,150** | **8.2%** | **0.89** |

> **Random Forest** was chosen as the best model because it achieves the highest **R² Score (0.89)** and lowest error metrics while capturing non-linear patterns.

---

## 🔎 Key Findings

| Indicator | Finding |
|-----------|---------|
| **Seasonality** | Strong weekly pattern — weekends show 20% higher sales |
| **Trend** | Consistent upward trend — 5% growth per quarter |
| **Holidays** | Holiday spikes increase sales by 30-40% |
| **Promotions** | Promotions boost sales by 20-30% |
| **Lag Features** | Previous week's sales are strong predictors |

---

## 📊 Visualizations

The notebook includes comprehensive visualizations:

- **Sales Over Time** — Daily and monthly trends
- **Seasonal Decomposition** — Trend, seasonal, residual components
- **Distribution Analysis** — Sales histogram and box plots
- **Day of Week Analysis** — Average sales by weekday
- **Feature Importance** — Top predictive features
- **Actual vs Predicted** — Model comparison
- **30-Day Forecast** — Future sales prediction with confidence interval

---

## 🚀 Quick Start

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels joblib
```

### 1. Run the Notebook

Open `sales_forecasting.ipynb` in Jupyter Lab / VS Code for the complete step-by-step analysis with visualizations.

### 2. Train the Model

```python
# The notebook will automatically:
# - Load and explore the data
# - Decompose time series components
# - Engineer features (lags, rolling stats)
# - Train 2 different models
# - Evaluate and compare performance
# - Generate 30-day forecast
```

### 3. Use the Saved Model

```python
import joblib

# Load the saved model
model = joblib.load('models/sales_forecast_model.pkl')

# Make predictions on new data
predictions = model.predict(future_features)
```

---

## 📁 Project Structure

```
sales-forecasting/
├── sales_forecasting.ipynb           # Jupyter notebook (full analysis)
├── requirements.txt                  # Python dependencies
├── models/
│   └── sales_forecast_model.pkl     # Trained Random Forest model
└── README.md
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python 3.10+ | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Basic plotting |
| Seaborn | Statistical visualization |
| Statsmodels | Time series analysis |
| Scikit-learn | ML models & preprocessing |
| Joblib | Model serialization |

---

**Built with Python, Statsmodels, Scikit-learn & Pandas**

[![GitHub stars](https://img.shields.io/github/stars/basitali08/sales-forecasting?style=social)](https://github.com/basitali08/sales-forecasting) [![GitHub forks](https://img.shields.io/github/forks/basitali08/sales-forecasting?style=social)](https://github.com/basitali08/sales-forecasting)

---

**Built by Basit Ali** · [GitHub](https://github.com/basitali08) · [Email](mailto:whoisbasit@gmail.com)  
Time Series & Forecasting Machine Learning · MS Data Science Portfolio
