✅ Project Plan: Energy Price Forecasting with Time Series
🔹 Objective
Predict day-ahead electricity prices using open data from Nord Pool or Fingrid.

🔹 Tools & Tech
Databricks (for data handling, modeling, and dashboarding)

Python (Pandas, Prophet or XGBoost)

MLflow (for experiment tracking)

Plotly/Seaborn or Databricks SQL Dashboard (for visualization)


1. Data Ingestion
Source: Download CSV from Nord Pool or use Fingrid API (they have open APIs).

Load it into Databricks using pandas or spark.read.

2. Exploratory Data Analysis
Plot daily and weekly price trends.

Check seasonality (daily, weekly, annual).

Visualize holidays or special events if available.

3. Feature Engineering
Add lag features (e.g., yesterday’s price).

Add rolling averages (7-day, 30-day).

Encode day of week, month, holiday flags.

4. Modeling
Choose one:

Prophet: Fast for univariate time series, auto seasonality detection.

XGBoost: With feature engineering, powerful for structured time series.

Compare both if time allows.

5. Forecasting
Predict next 7 or 14 days of electricity prices.

Include confidence intervals.

Decompose seasonality if using Prophet.

6. Visualization
Use Databricks Dashboard (via display widgets or SQL Dashboard) to show:

Actual vs. Predicted

Seasonality

Confidence intervals

Bonus: Interactive model retraining widget (date picker, look-back period).

7. Insights
Share 2–3 insights about energy pricing patterns.

Explain what would happen in a battery optimization context (e.g., when to buy/store/sell based on forecast).
