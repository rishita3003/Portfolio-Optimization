# Portfolio-Optimization
## Overview
This project focuses on the risk assessment and optimization of stock portfolios using historical data. The primary goal is to maximize the Sharpe ratio, which indicates the best possible return-to-risk scenario for a given portfolio.

## Features
- **Risk Assessment**: Analyze stocks based on their historical volatility and returns.
- **Sharpe Ratio Calculation**: Compute the Sharpe ratio to identify the most efficient portfolio.
- **Visualization**: Plot risk-return profiles to visually assess potential investment choices.

## Technologies Used
- **Python Library**
   - _**Pandas**_ for data manipulation
   - _**NumPy**_ for numerical calculations
   - _**Matplotlib**_ and Seaborn for data visualization
   - _**Yahoo Finance**_ for fetching historical stock data

## Getting Started
To run this project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/rishita3003/Portfolio-Optimization.git
   ```

2. **Install required Python libraries**:
    ```bash
   pip install pandas numpy matplotlib seaborn yfinance
    ```

4. **Execute the Jupyter notebook**:
   ```bash
   jupyter notebook "portfolio optimization.ipynb"
   ```

## Overview
This Jupyter notebook orchestrates a series of data processing and analysis steps to optimize stock portfolios. Each step builds on the previous to methodically advance toward determining the most efficient portfolio configuration.

## Architecture Steps

### 1. Data Fetching
- **Objective:** Collect historical closing prices of selected stocks.
- **Tools Used:**
  - Yahoo Finance API
  - `yfinance` Python library
- **Process:**
  - Fetch closing prices for a predefined list of stocks over a specified date range.
  - This data is foundational for subsequent analysis steps.

### 2. Returns Calculation
- **Objective:** Calculate daily logarithmic returns of the stocks.
- **Methodology:**
  - Logarithmic returns are used for their numerical stability and time-additivity.
- **Process:**
  - Calculate returns using `log(price_today / price_yesterday)`.

### 3. Portfolio Simulation
- **Objective:** Simulate various portfolio weight allocations to evaluate potential investment strategies.
- **Tools Used:** NumPy for numerical computations.
- **Process:**
  - Generate thousands of random portfolio weight combinations (totaling 1).
  - For each combination, compute the portfolio's expected return and risk.

### 4. Optimization Output
- **Objective:** Identify the optimal portfolio configuration with the highest Sharpe ratio.
- **Tools Used:**
  - Matplotlib for plotting
  - NumPy for calculations
- **Process:**
  - Determine the portfolio with the best risk-adjusted return.
  - Present this portfolio through tables and a graphical efficient frontier.

### 5. Visualization and Conclusion
- **Objective:** Visualize and conclude the analysis.
- **Tools Used:**
  - Matplotlib and Seaborn for visual representation
- **Process:**
  - Display scatter plots of simulated portfolios on a risk-return plane.
  - Highlight the efficient frontier and the optimal portfolio.

## Conclusion
This structured approach ensures systematic analysis and supports clear decision-making, making the notebook a reusable and adaptable tool for portfolio optimization tasks.



## Results
- Visualizations of the efficient frontier demonstrate the trade-off between risk and return.
- The optimal portfolio configuration and its expected annual return and risk metrics are presented.
## Conclusion
This project successfully demonstrates how to apply quantitative techniques to optimize stock portfolios, maximizing returns while controlling for risk.



   

