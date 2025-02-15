Trading Account Performance Analysis
Project Overview
This project analyzes trade history data to calculate key metrics for trading accounts. The metrics include ROI, PnL (Profit and Loss), Win Rate, Sharpe Ratio, and Maximum Drawdown (MDD). The objective is to evaluate the performance of each account over a 90-day period and rank the accounts based on their ROI.

Dataset
The dataset used for this analysis is a CSV file, TRADES_CopyTr_90D_ROI.csv, which contains historical trade data with a Trade_History column. Each entry in the Trade_History is a list of trades for a specific account, including details like realized profit, quantity traded, and more.

Approach
Load Dataset: The CSV file is read into a Pandas DataFrame.
Parse Trade History: The Trade_History column is parsed into a list of dictionaries using AST.
Calculate Metrics: Metrics like ROI, PnL, Sharpe Ratio, MDD, and Win Rate are calculated for each account.
Rank Accounts: Accounts are ranked based on ROI and the top 20 accounts are extracted.
Generate Output: The results are saved into account_metrics.csv and the top 20 ranked accounts are saved into top_20_accounts.csv. A detailed report is also generated.
Files
TRADES_CopyTr_90D_ROI.csv: Input dataset.
account_metrics.csv: Output file containing performance metrics for each account.
top_20_accounts.csv: Output file containing the top 20 accounts ranked by ROI.
report.txt: A summary report outlining the methodology and findings.
Requirements
Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
AST: For parsing string representations of lists/dictionaries.
How to Run
Clone the repository:

bash
Copy
git clone https://github.com/yourusername/trading-account-analysis.git
Install the required dependencies:

nginx
Copy
pip install pandas numpy
Run the script:

nginx
Copy
python analyze_trading_data.py
Check the results in account_metrics.csv, top_20_accounts.csv, and report.txt.

Insights
The project calculates and ranks accounts based on ROI, helping identify top-performing traders.
