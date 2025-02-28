# Mutual Fund Plan with Python

## Overview
This project demonstrates how to create a mutual fund plan by analyzing stock market data using Python. It involves gathering historical stock data, calculating key financial metrics, and selecting stocks based on return on investment (ROI) and volatility.

## Features
- Load and process historical stock data
- Calculate ROI and volatility
- Identify stocks with high ROI and low risk
- Allocate investments using inverse volatility ratio
- Compare mutual fund risk and ROI against high-growth companies
- Visualize stock price trends, risk comparison, ROI comparison, and future value calculations
- Generate insights for investment strategies

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/mutual-fund-plan.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mutual-fund-plan
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Run the Python script to analyze stock data and generate investment insights:
```bash
python mutual_fund.py
```

## Methodology & Analysis
### 1. Data Collection
- Historical stock data is loaded into a Pandas DataFrame.
- The dataset includes stock prices, ROI, and volatility measures.

### 2. Stock Selection
- Stocks are filtered based on high ROI and low volatility.
- Selected stocks include ICICI Bank, IndusInd Bank, JSW Steel, Axis Bank, HDFC Bank, Sun Pharma, Kotak Bank, Cipla, and NTPC.

### 3. Investment Allocation
- Investment is allocated using the **inverse volatility ratio**.
- Companies with lower volatility receive a higher weight in the portfolio.

### 4. Risk Comparison
- The volatility of selected mutual fund stocks is compared to high-growth companies.
- A bar chart visualizes the comparison, showing lower risk for mutual fund stocks.

### 5. ROI Comparison
- The expected ROI of selected mutual fund stocks is compared to high-growth companies.
- A bar chart demonstrates the trade-off between risk and return.

### 6. Expected Returns Calculation
- Monthly investments of ₹5000 are simulated for 1, 3, 5, and 10 years.
- Future value is calculated using compound interest formula:
  ```python
  def future_value(P, r, n, t):
      return P * (((1 + r/n)**(n*t) - 1) / (r/n)) * (1 + r/n)
  ```
- The projected investment value is visualized with a line chart.

## Visualizations
- **Risk Comparison Graph:** A bar chart comparing volatility between mutual fund companies and high-growth stocks.
- **ROI Comparison Graph:** A bar chart comparing expected ROI between mutual fund and high-growth stocks.
- **Future Investment Growth Graph:** A line chart showing the accumulated value of investments over different time periods.

## Dependencies
- Python 3.x
- Pandas
- Plotly
- NumPy

## Dataset
The project uses a historical stock price dataset. Ensure you have the dataset stored in the project directory before running the analysis.

## Contribution
Feel free to contribute by submitting issues or pull requests.
