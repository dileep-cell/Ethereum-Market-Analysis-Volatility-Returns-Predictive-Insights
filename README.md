# 🪙 Ethereum (ETH–USD) Market Analysis & Price Forecasting

## 📌 Project Overview

**Motto:** "Understand the market before you predict it."

This project delivers an end-to-end analytical deep dive into the Ethereum (ETH–USD) market, combining exploratory data analysis, risk metrics, advanced market diagnostics, and machine learning–based price forecasting. The analysis provides actionable market insights and short-term price forecasts using a structured, data-driven approach.

Instead of jumping straight into modeling, this project prioritizes data quality, market behavior, and risk awareness, ensuring forecasts are grounded in reality—not just algorithms.

## 📂 Data Source & Dataset Details

**Primary Source:** [CoinGecko](https://www.coingecko.com/)

- Platform: Kaggle
- Dataset: Ethereum historical market data (ETH–USD)

### Dataset Type
- Time-series financial market data
- Granularity: Daily observations
- Nature: Historical, numerical, multivariate

### Key Features
- Timestamp (snapped_at)
- Price metrics (open, high, low, close)
- Market capitalization
- Trading volume

## 🧹 Data Preparation & Feature Engineering

Before analysis, the dataset undergoes a rigorous preprocessing pipeline:

✅ Structure validation: data types, ranges, and schema checks

✅ Data quality checks: null, NaN, and infinite value detection

✅ Timestamp handling:
- Converted from UTC to IST (Asia/Kolkata) for localized analysis
- Set as time-series index

✅ Feature extraction:
- Date, hour, weekday, and month derived for temporal insights

This ensures the dataset is clean, reliable, and analysis-ready.

## 📈 Exploratory Data Analysis (EDA)

A comprehensive EDA phase uncovers market behavior and volatility patterns:

### Market Overview
- Current, high, low, average prices
- Price range and spread analysis

### Performance Metrics
- Total return over the period
- Average daily return
- Best & worst trading days
- Win-rate (positive return days)

### Risk Metrics
- Daily and rolling volatility
- Maximum drawdown
- Extreme return detection

### Market Activity
- Market capitalization trends
- Trading volume analysis
- Price–volume relationships and lead–lag effects

**Result:** A clear picture of Ethereum's risk-return profile and trading dynamics.

## 🧠 Advanced Analytics

To move beyond surface-level insights, the project explores:
- Volatility regime identification
- Detection of abnormal price and volume spikes
- Return distribution behavior under different market conditions

This step bridges the gap between descriptive analytics and predictive modeling.

## 🤖 Machine Learning–Based Price Forecasting

### Models Used
- XGBoost (Extreme Gradient Boosting)
- LightGBM (Light Gradient Boosting Machine)

### Modeling Approach
- Lag-based and historical feature construction
- Supervised regression framework
- Evaluation using error metrics (e.g., MAE, RMSE)
- Forward-looking price projections on unseen future dates

### Why These Models?
- Handle non-linearity and market noise effectively
- Perform well on structured time-series data
- Widely adopted in real-world financial forecasting

## 📊 Model Results & Performance Metrics

### Raw Model Performance
| Model | MAE ($) | RMSE ($) | Performance |
|-------|---------|----------|-------------|
| **LightGBM** | 179.28 | 236.53 | ⭐ Superior |
| **XGBoost** | 197.92 | 251.35 | — |

**Key Finding:** LightGBM outperforms XGBoost by **9.4% on MAE** and **5.8% on RMSE**, demonstrating superior accuracy in predicting short-term price movements.

---

### 🔍 Real-Time Validation: 20-Day Live Accuracy

**Data Source:** [Investing.com Ethereum Historical Data](https://www.investing.com/crypto/ethereum/historical-data)

**Performance Summary:**
- LightGBM achieved **3 near-perfect predictions** (APE: 0.03%, 0.32%, 1.95%)
- XGBoost hit accurate range only **1 day** during same period
- Both models struggle during **sharp volatility** (Oct 3–6 drawdown), overestimating by 15–25%

**Key Wins:**
| Date | LightGBM APE | Status |
|------|--------------|--------|
| Oct 17 | 0.03% | **Near-Perfect** |
| Oct 18 | 0.32% | **Strong Hit** |

**Where Both Miss:**
- Systematic overestimation during crash periods (Oct 3–6)
- XGBoost shows "prediction inertia"—same predicted value (~$3,764.96) for 8+ consecutive days
- Both lag in capturing volatility shocks

**📌 Critical Insight:** LightGBM recovers **3x faster** after volatility spikes than XGBoost.

### 🏁 Bottom-Line Executive Verdict

| Metric | Winner | Implication |
|--------|--------|------------|
| **Overall Accuracy** | LightGBM | 9.4% better MAE |
| **Volatility Handling** | LightGBM | Faster crash recovery |
| **Consistency** | LightGBM | Lower error variance |
| **Crash Sensitivity** | ⚠️ Both Models | Need ensemble approach for black swan events |

**Recommendation:** LightGBM is production-ready for short-term (1–3 day) forecasting. For longer horizons or extreme volatility, recommend ensemble methods or adding external sentiment data.

## 📌 Final Inference & Key Takeaways

Ethereum exhibits high volatility with distinct risk regimes, making naive forecasting unreliable.

Strong relationships exist between price movements, trading volume, and volatility spikes.

Gradient boosting models (XGBoost & LightGBM) demonstrate robust short-term forecasting capability when supported by proper feature engineering.

The project emphasizes that model performance improves significantly when market behavior is well understood beforehand.

## 🚀 Skills Demonstrated

- Time-series analysis & financial metrics
- Data cleaning & feature engineering
- Exploratory data analysis (EDA)
- Risk & volatility assessment
- Machine learning with XGBoost & LightGBM

### Key Analyses Performed
- 30-day rolling volatility & volatility distribution analysis
- Trading volume trends and volume distribution
- Price distribution and historical price movement analysis
- Feature correlation analysis to identify predictive drivers
- Price action study using moving averages
- Daily returns computation and distribution analysis
- Volatility-aware forecasting using XGBoost and LightGBM
- Visual comparison of actual vs predicted price movements
- Analytical storytelling with business relevance

📊 Deep dive into model results (Full 20-Day Model Accuracy & Miss Breakdown)
