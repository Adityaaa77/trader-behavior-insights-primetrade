Trader Behavior and Performance Analysis

Primetrade.ai – Data Science / Analytics Intern Assignment

Project Overview

This project analyzes historical trader behavior and performance on the Hyperliquid platform. The objective is to evaluate trading outcomes, behavioral patterns, and risk characteristics using structured data analysis. The original scope included analyzing the relationship between market sentiment (Bitcoin Fear and Greed Index) and trader performance. During the analysis, a temporal mismatch between datasets was identified and handled transparently to ensure analytical correctness.

The submission emphasizes data validation, aggregation, behavioral insights, and actionable strategy recommendations aligned with real-world data science practices.

Datasets Used

Bitcoin Fear and Greed Index

Daily market sentiment classifications (Fear, Greed, Neutral)

Hyperliquid Historical Trader Data

Trade-level data including execution details, position size, PnL, side, and timestamps

Important Note:
The available Hyperliquid trade data is concentrated in December 2024, while the provided Fear and Greed Index dataset does not temporally overlap with these trade dates. This limitation was identified and documented, and sentiment-based analysis was not forced to avoid invalid temporal joins.

Data Preparation and Feature Engineering

Key preprocessing steps include:

Parsing and standardizing timestamps

Validating date ranges across datasets

Aggregating trade data to a daily per-trader level

Creating core performance metrics:

Daily PnL

Trade frequency

Average trade size

Buy and sell trade counts

Win rate

All data cleaning and transformations are fully documented in the notebook.

Key Insights

Profitability is skewed: A small number of high-PnL outcomes disproportionately influence average returns, while median daily PnL remains significantly lower.

Trade frequency varies widely: Excessive trading does not consistently translate into higher profitability, indicating potential overtrading risk.

Win rate is relatively strong: Despite a healthy overall win rate, large negative PnL events highlight the importance of risk management and position sizing discipline.

Strategy Recommendations

Risk control for high-frequency traders
Traders with high daily trade counts should enforce stricter position sizing or stop-loss limits to prevent large drawdowns that negate cumulative gains.

Focus on consistency over volume
Emphasizing high-conviction trades rather than increasing trade frequency can improve risk-adjusted performance.

Forward-looking sentiment integration
With overlapping sentiment data, exposure adjustments could be made based on Fear and Greed regimes, particularly for high-risk trader segments.

How to Run

Clone the repository

Place datasets in the data/ directory

Open notebook.ipynb using Jupyter Notebook or VS Code

Run all cells sequentially

Notes on Reproducibility

All analysis steps are deterministic and reproducible

No external APIs are required

Dataset limitations are explicitly documented

Author

Aditya
Data Science Intern Applicant
