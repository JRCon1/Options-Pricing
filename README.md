# Options-Pricing
Options Pricing Simulation using Python (Black-Scholes &amp; Monte Carlo)

***Overview***

This tool provides a streamlined and interactive approach for analyzing options data. It leverages financial models and data science techniques to calculate key metrics such as Greeks, intrinsic value, extrinsic value, and theoretical pricing using the Black-Scholes Model (BSM) and Monte Carlo simulations.

**Features:**

- Dynamic Filtering: Filter options by strike price and expiration date based on user-defined bounds.

- Option Metrics: Calculate Greeks (Delta, Gamma, Vega, Theta, Rho) and key financial metrics (Intrinsic Value, Premium per Day, Return on Capital).
- Pricing Models:
    - Black-Scholes Model (BSM)
    - Monte Carlo Simulations

- Interactive Inputs: Easily adjust parameters like ticker symbol, option type, and strike price bounds.

- Optimized Data Presentation: Analyze filtered data for accuracy and actionable insights.


**Getting Started**

*Prerequisites*
- Python 3.x
- Google Colab (optional but recommended for seamless execution)

*Required Libraries* :
- pandas
- numpy
- yfinance
- py_vollib
- scipy

**Install the necessary libraries using:**
- pip install pandas numpy yfinance py_vollib scipy

**Running the Tool**

1.) Clone the repository:
- git clone <repository_url>

2.) Navigate to the project directory and open the script in your preferred environment.

3.) Execute the script step-by-step, providing inputs as prompted:
- Upper and Lower Bound: Enter the percentage bounds for strikes as a decimal (e.g., 0.20 for 20%).
- Ticker Symbol: Enter the stock ticker symbol (e.g., AAPL).
- Option Type: Enter c for call or p for put.

**Outputs**

The tool outputs a Pandas DataFrame containing the following:
- Strike Prices: Range of filtered options.
- Mid-Point Price: Average of the bid-ask spread.
- BSM Price: Theoretical price using the Black-Scholes Model.
- Monte Carlo Price: Theoretical price from Monte Carlo simulations.
- Days to Expiry: Remaining time until expiration.

**Customization**

- Risk-Free Rate: Modify the r variable at the start of the script to use a different risk-free rate.
- Greeks Calculation: Adjust the greeks() function for additional metrics or alternative formulas.
- Monte Carlo Simulations: Change the number of simulations (n) in the monte_carlo_price() function for greater accuracy or faster computation.

**Example Use Case**

# Sample Execution:
Enter the upper & lower bound for strikes as a decimal (Ex: 0.20 for 20%): 0.10
Enter the ticker symbol: AAPL
Enter the option type (c for call, p for put): c

**Outputs a filtered DataFrame with:**

- The tool outputs a Pandas DataFrame containing the following:

  - Strike: 180
  - Mid-Point Price: 2.35
  - BSM Price: 2.30
  - Monte Carlo Price: 2.33
  -Days To Expiry: 30

**Contributions**

Feel free to submit issues or pull requests to improve functionality. Collaboration is welcome for:
- Additional pricing models (e.g., Binomial Tree).
- Improved user interface & any other UI design for similar projects.
-  Integration with external data sources for further pricing.

**License**

- This project is licensed under the MIT License. See the LICENSE file for details.

**Acknowledgments**

- Libraries Used:

  - py_vollib for Greek calculations

  - yfinance for historical data

  - scipy for statistical functions

**References:**

- Black-Scholes Model: Wikipedia

- Monte Carlo Methods: Investopedia

**Contact**

For questions or feedback, please reach out to the project maintainer.
jr1concepcion@gmail.com
