# Cryptocurrency-Database-Prediction-


Multi-Asset Market Analysis Pipeline
A Python-based data analysis tool that interfaces with a SQLite database to compare volatility and return correlations between cryptocurrencies (ETH, SOL) and traditional market indices (NASDAQ, S&P 500).

📊 Project Overview
This project automates the extraction and visualization of market data to answer a key financial question: How closely does the crypto market track traditional tech stocks?

The pipeline performs the following:

Data Extraction: Queries an SQLite database using complex SQL JOIN operations to align disparate asset time series by date.

Statistical Analysis: Calculates 7-day rolling volatility and daily return correlations (Pearson correlation) between assets.

Data Visualization: Generates a high-resolution bar chart comparing volatility across asset classes, including Gold and Crude Oil.

🛠️ Tech Stack
Language: Python 3.x

Database: SQLite

Libraries: * Pandas: Data manipulation and SQL integration.

Matplotlib: Professional-grade data visualization.

Pathlib: Cross-platform file path management.

📈 Key Insights Captured
The script generates several summary reports, including:

Volatility Rankings: Identifying which assets carry the highest risk profile.

Asset Correlations: Measuring the "decoupling" or coupling of ETH/SOL vs. the NASDAQ.

Return Summaries: Minimum, maximum, and average daily returns across all tracked assets.

🚀 Getting Started
Prerequisites
Ensure you have the following installed:

Bash
pip install pandas matplotlib
Setup
Clone this repository:

Bash
git clone https://github.com/your-username/market-data-analysis.git
Place your market_data.db in the root directory (the script uses Pathlib to locate it automatically).

Run the analysis:

Bash
python analysis_script.py
🖼️ Visualizations
The script exports a high-quality visualization (volatility_chart.png) comparing the risk profiles of different asset classes:

Example output:

📁 Repository Structure
Plaintext
├── market_data.db       # SQLite database (not included in repo)
├── analysis.py          # Main Python analysis script
├── volatility_chart.png # Generated output chart
└── README.md            # Project documentation
