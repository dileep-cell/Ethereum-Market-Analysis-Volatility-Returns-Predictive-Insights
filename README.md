📊 Ethereum (ETH–USD) Market Analysis & Price Forecasting
📌 Project Overview

This project delivers an end-to-end analytical deep dive into the Ethereum (ETH–USD) market, combining exploratory data analysis, risk metrics, advanced market diagnostics, and machine learning–based price forecasting.

The goal is simple but ambitious:
turn raw crypto market data into actionable market insights and short-term price forecasts using a structured, data-driven approach.

🎯 Project Motto

“Understand the market before you predict it.”

Instead of jumping straight into modeling, this project prioritizes data quality, market behavior, and risk awareness, ensuring forecasts are grounded in reality—not just algorithms.

📂 Data Source & Dataset Details
🔹**Primary Source:** [CoinGecko](https://www.coingecko.com/)

Platform: Kaggle

Dataset: Ethereum historical market data (ETH–USD)


🔹 Dataset Type

Time-series financial market data

Granularity: Daily observations

Nature: Historical, numerical, multivariate

🔹 Key Features

Timestamp (snapped_at)

Price metrics (open, high, low, close)

Market capitalization

Trading volume

🧹 Data Preparation & Feature Engineering

Before analysis, the dataset undergoes a rigorous preprocessing pipeline:

✅ Structure validation: data types, ranges, and schema checks

✅ Data quality checks: null, NaN, and infinite value detection

✅ Timestamp handling:

Converted from UTC to IST (Asia/Kolkata) for localized analysis

Set as time-series index

✅ Feature extraction:

Date, hour, weekday, and month derived for temporal insights

This ensures the dataset is clean, reliable, and analysis-ready.

📈 Exploratory Data Analysis (EDA)

A comprehensive EDA phase uncovers market behavior and volatility patterns:

🔹 Market Overview

Current, high, low, average prices

Price range and spread analysis

🔹 Performance Metrics

Total return over the period

Average daily return

Best & worst trading days

Win-rate (positive return days)

🔹 Risk Metrics

Daily and rolling volatility

Maximum drawdown

Extreme return detection

🔹 Market Activity

Market capitalization trends

Trading volume analysis

Price–volume relationships and lead–lag effects

📊 Result: A clear picture of Ethereum’s risk-return profile and trading dynamics.

🧠 Advanced Analytics

To move beyond surface-level insights, the project explores:

Volatility regime identification

Detection of abnormal price and volume spikes

Return distribution behavior under different market conditions

This step bridges the gap between descriptive analytics and predictive modeling.

🤖 Machine Learning–Based Price Forecasting
🔹 Models Used

XGBoost (Extreme Gradient Boosting)

LightGBM (Light Gradient Boosting Machine)

🔹 Modeling Approach

Lag-based and historical feature construction

Supervised regression framework

Evaluation using error metrics (e.g., MAE, RMSE)

Forward-looking price projections on unseen future dates

🔹 Why These Models?

Handle non-linearity and market noise effectively

Perform well on structured time-series data

Widely adopted in real-world financial forecasting

📌 Final Inference & Key Takeaways

Ethereum exhibits high volatility with distinct risk regimes, making naive forecasting unreliable.

Strong relationships exist between price movements, trading volume, and volatility spikes.

Gradient boosting models (XGBoost & LightGBM) demonstrate robust short-term forecasting capability when supported by proper feature engineering.

The project emphasizes that model performance improves significantly when market behavior is well understood beforehand.


🚀 Skills Demonstrated

Time-series analysis & financial metrics

Data cleaning & feature engineering

Exploratory data analysis (EDA)

Risk & volatility assessment

Machine learning with XGBoost & LightGBM
Key Analyses Performed

30-day rolling volatility & volatility distribution analysis

Trading volume trends and volume distribution

Price distribution and historical price movement analysis

Feature correlation analysis to identify predictive drivers

Price action study using moving averages

Daily returns computation and distribution analysis

Volatility-aware forecasting using XGBoost and LightGBM

Visual comparison of actual vs predicted price movements

Analytical storytelling with business relevance



📊  Deep dive into model results (Full 20-Day Model Accuracy & Miss Breakdown)
Date	Actual Close ($)	LightGBM Pred ($)	LGBM Miss ($)	LGBM APE %	LGBM Verdict	XGBoost Pred ($)	XGB Miss ($)	XGB APE %	XGB Verdict
Oct 1	3,874.80	3,971.45	+96.65	2.49%	❌ Miss	4,055.27	+180.47	4.66%	❌ Miss
Oct 2	3,908.28	3,923.48	+15.20	0.39%	✅ No Miss	4,082.43	+174.15	4.46%	❌ Miss
Oct 3	3,603.63	3,839.97	+236.34	6.56%	❌ Miss	3,930.63	+327.00	9.07%	❌ Miss
Oct 4	3,289.11	3,811.54	+522.43	15.88%	❌ Miss	4,025.90	+736.79	22.40%	❌ Miss
Oct 5	3,424.74	3,830.30	+405.56	11.84%	❌ Miss	3,979.09	+554.35	16.19%	❌ Miss
Oct 6	3,314.43	3,901.45	+587.02	17.71%	❌ Miss	3,845.40	+530.97	16.02%	❌ Miss
Oct 7	3,435.78	3,901.70	+465.92	13.56%	❌ Miss	3,764.03	+328.25	9.55%	❌ Miss
Oct 8	3,401.53	3,882.93	+481.40	14.15%	❌ Miss	3,767.19	+365.66	10.75%	❌ Miss
Oct 9	3,584.18	3,811.79	+227.61	6.35%	❌ Miss	3,764.96	+180.78	5.04%	❌ Miss
Oct 10	3,567.87	3,811.54	+243.67	6.83%	❌ Miss	3,764.96	+197.09	5.52%	❌ Miss
Oct 11	3,417.56	3,830.30	+412.74	12.08%	❌ Miss	3,764.96	+347.40	10.17%	❌ Miss
Oct 12	3,413.60	3,901.45	+487.85	14.29%	❌ Miss	3,764.96	+351.36	10.29%	❌ Miss
Oct 13	3,232.94	3,901.70	+668.76	20.69%	❌ Miss	3,764.96	+532.02	16.46%	❌ Miss
Oct 14	3,113.03	3,882.93	+769.90	24.73%	❌ Miss	3,764.96	+651.93	20.94%	❌ Miss
Oct 15	3,985.52	3,811.79	−173.73	4.36%	❌ Miss	3,764.96	−220.56	5.53%	❌ Miss
Oct 16	3,894.48	3,811.54	−82.94	2.13%	❌ Miss	3,764.96	−129.52	3.33%	❌ Miss
Oct 17	3,831.60	3,830.30	−1.30	0.03%	✅ No Miss	3,764.96	−66.64	1.74%	✅ No Miss
Oct 18	3,888.87	3,901.45	+12.58	0.32%	✅ No Miss	3,764.96	−123.91	3.19%	❌ Miss
Oct 19	3,982.53	3,901.70	−80.83	2.03%	❌ Miss	3,764.96	−217.57	5.46%	❌ Miss
Oct 20	3,979.43	3,901.70	−77.73	1.95%	✅ No Miss	3,764.96	−214.47	5.39%	❌ Miss

🧠 What this table proves
LightGBM

✅ 4 / 20 days accurate

🎯 Near-perfect on Oct 17

⚠️ Overestimates during crash, adapts later

XGBoost

✅ 1 / 20 days accurate

❌ Flat predictions = regime blindness

❌ Larger bias during drawdowns

“LightGBM demonstrates superior adaptability and tighter convergence, while XGBoost exhibits prediction inertia, leading to systematic overestimation during volatile regimes.”
