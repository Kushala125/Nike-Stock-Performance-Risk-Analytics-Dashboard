Strategic Financial Analysis: Nike Inc. (NKE) Market Intelligence & Quantitative Modeling
1. Executive Mission Statement
The objective of this comprehensive study is to transform 25 years of raw Nike (NKE) historical stock data into a strategic roadmap for investment decision-making. In a market characterized by high noise and cyclicality, this project utilizes a high-performance data stack—comprising SQL, Python, and Tableau—to engineer features that distinguish market signals from random fluctuations. The ultimate goal is to provide a data-backed evaluation of risk-adjusted returns and the efficacy of algorithmic trading vs. traditional asset management.

2. Technical Architecture & Methodology
To ensure the highest level of analytical rigor, a multi-disciplinary technical approach was implemented:

A. Data Engineering & Schema Optimization (SQL)
The foundation of the project rests on advanced data manipulation within a relational database environment.

Temporal Normalization: Developed custom scripts using STR_TO_DATE to convert legacy string formats into standardized ISO-8601 datetime objects, enabling complex time-series queries.

Window Function Implementation: Leveraged LAG() and LEAD() functions to calculate inter-day price delta and percentage returns, essential for measuring daily market momentum.

Rolling Aggregations: Utilized AVG() OVER with specific frame clauses (ROWS BETWEEN 49 PRECEDING AND CURRENT ROW) to calculate 50-day moving averages directly within the database layer for maximum efficiency.

B. Quantitative Analysis & Feature Engineering (Python)
Using the Jupyter ecosystem, the raw data was subjected to rigorous statistical testing:

Exploratory Data Analysis (EDA): Performed distribution analysis on trading volume and price spreads to identify anomalies and historical outliers.

Technical Indicator Development: Engineered the Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) logic to define "Overbought" and "Oversold" market conditions.

Volatility Modeling: Calculated rolling standard deviations of returns to identify periods of "Volatility Clustering," providing a quantitative metric for market risk.


How can we use data to determine whether Nike stock is a good investment and when to buy or sell it?

C. Strategic Visualization (Tableau)
To bridge the gap between technical output and executive understanding:

Dynamic Dashboards: Developed an interactive Tableau workbook that visualizes the relationship between volume spikes and price reversals.

Trend Decomposition: Created visual overlays of short-term (50-day) vs. long-term (200-day) moving averages to highlight "Golden Cross" and "Death Cross" events in Nike’s history.

3. Critical Business Insights & Strategic Findings
The analysis moved beyond descriptive statistics to provide high-level business intelligence:

The 2021 Peak & Correction: The data identifies November 2021 as a historical high-water mark for NKE. The subsequent decline was not a random event but a structured "Market Correction" phase. Recognizing these patterns allows for better timing of capital entry and exit.

Algorithmic Strategy Evaluation: A core component of the project was backtesting a Moving Average Crossover strategy.

Finding: While the strategy maintained a win rate exceeding 50%, it ultimately underperformed a "Buy and Hold" strategy over a 20-year horizon.

Strategy Recommendation: For high-growth assets like Nike, the data suggests that "Market Timing" often incurs higher transaction costs and missed upside compared to "Time in the Market."

Volatility as a Risk Signal: The analysis detected that "High Volatility" days (price swings > 3%) often cluster during specific economic cycles. This insight is vital for institutional risk management and setting stop-loss parameters.

4. Professional Challenges & Solutions
A key indicator of high-level expertise is the ability to overcome complex data hurdles:

Challenge: Data Type Inconsistency.

Solution: The original dataset lacked proper formatting for time-series analysis. I implemented a programmatic fix in the Python ETL pipeline to ensure all 6,559 records were indexed by time, ensuring the validity of all subsequent rolling calculations.

Challenge: Signal Noise in Daily Returns.

Solution: Daily price movements are often erratic. I implemented "Smoothing Functions" through moving averages to extract the underlying trend, allowing for a clearer view of Nike’s long-term value proposition.

5. Professional Conclusion
This project serves as a definitive demonstration of the intersection between Data Science and Financial Strategy. By successfully managing the full data lifecycle—from ingestion and cleaning to advanced modeling and visual storytelling—this analysis provides a blueprint for evidence-based decision-making.

The findings emphasize that while technical analysis tools like RSI and Moving Averages are powerful for risk mitigation, the long-term fundamentals of Nike Inc. support a structured investment approach. This study proves a readiness to handle large-scale financial datasets and translate them into the clear, actionable narratives required for executive-level leadership and institutional growth.

6. Technical Skills Demonstrated
Languages: SQL (MySQL), Python (Pandas, NumPy, Matplotlib, Seaborn)

Tools: Tableau Desktop, Jupyter Notebooks, Excel/CSV Data Engineering

Finance Competencies: Time-Series Forecasting, Technical Indicator Development, Risk/Return Analysis, Backtesting Methodologies, Market Cycle Identification.
