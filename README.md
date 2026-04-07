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
1. How can data-driven analysis of historical stock performance be used to evaluate return, risk, and strategy effectiveness for investment decision-making?
   ![chart](images/chart1.png)
   ![chart](images/chart2.png)
 Insights
## The dataset used in this analysis consists of 6,559 records spanning from January 3, 2000 to January 30, 2026, providing a comprehensive long-term view of stock price behavior. 

It includes key financial variables such as open, close, high, low prices, trading volume, and several engineered features like moving averages, RSI, MACD, and machine learning signals
.
Over the observed period, the stock demonstrates a strong long-term upward trend, with the lowest recorded price at approximately 2.47 and the highest reaching 166.25, indicating significant growth potential over time.

The average closing price is around 42.20 with a high standard deviation, reflecting substantial volatility in price movements.

The average daily return is relatively small at approximately 0.06%, but the presence of extreme values, such as a maximum gain of 15.53% and a maximum loss of -19.98%, highlights the unpredictable and volatile nature of the market.

The best performing day occurred on June 25, 2021, where the stock experienced a sharp increase of over 15%, supported by strong momentum and high trading volume, with RSI values indicating an overbought condition. 

In contrast, the worst performing day was observed on June 28, 2024, with a nearly 20% decline, accompanied by extremely high trading volume and an RSI value indicating an oversold condition, suggesting panic selling or adverse market events.

Moving average indicators, particularly the 50-day and 200-day averages, were effective in identifying trends, where crossovers signaled bullish or bearish market conditions. 

Additional technical indicators such as RSI and MACD provided further insights into momentum and potential reversal points, enhancing the robustness of the analysis.

Several trading strategies were implemented, including basic moving average strategies, filtered signals, advanced strategies using RSI and MACD, and risk-controlled approaches using stop-loss and take-profit mechanisms.

These strategies demonstrated moderate profitability, with cumulative returns generally exceeding the baseline while managing risk more effectively than raw market exposure.


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
