VaR: The VaR value is interpreted as the maximum potential loss that is expected to occur with a certain confidence level over a given time horizon. For instance, a VaR of $100,000 at a 95% confidence level means that there is a 5% chance that the portfolio will lose more than $100,000 over the specified time horizon.


1. Portfolio_Risk_Management_Monte_Carlo

Monte Carlo simulation is a method that uses random sampling and statistical modeling to estimate complex phenomena or predict future outcomes. 
In the context of this code, it is being used to simulate portfolio returns and assess the risk metrics (VaR and CVaR) based on simulated data.

2. Portfolio_Risk_Management_Historical_Sim_Method

The Historical Method for assessing Value at Risk (VaR) is one of the simplest and most intuitive approaches to estimating potential losses in a portfolio over a specified time horizon, given the historical price data. It relies purely on the actual past returns of assets or a portfolio, without making any assumptions about the underlying distribution of returns. 

  Steps:
  1. Collect Historical Data: You start by collecting the historical data of the asset or portfolio you want to assess. This could be daily, weekly, or monthly returns,            depending on the time horizon of interest. The more data points you have, the more reliable the estimation is likely to be.

  2. Calculate Historical Returns: Once you have the historical price data, you calculate the returns. The return for each period (e.g., daily) is typically computed as the        percentage change in the price from one period to the next.

  3. Order the Returns: After calculating the returns for all periods, the next step is to sort these returns from worst to best (i.e., in ascending order).

  4. Determine the VaR Quantile: To calculate VaR at a given confidence level (e.g., 95% or 99%), you select the appropriate quantile from the sorted return distribution.
    For a 95% confidence level, you would look at the return that is greater than or equal to 5% of the worst returns (i.e., the 5th percentile).
    For a 99% confidence level, you would look at the return that is greater than or equal to 1% of the worst returns (i.e., the 1st percentile).
    For example, with a 95% confidence level, the VaR is the 5th percentile of the historical return distribution.



Advantages of the Historical VaR Method

  1. No Assumptions about Distribution: Unlike parametric methods (e.g., the Variance-Covariance method), the Historical VaR method doesn’t require assumptions about the           distribution of returns (e.g., normal distribution).

  2. Simple and Intuitive: It is straightforward to understand and easy to implement, as it relies on actual past market data.

  3. Reflects Real Market Conditions: Since it uses real historical data, it inherently captures the market’s past behavior, including extreme events, outliers, and                correlations between assets.

Disadvantages of the Historical VaR Method

  1. Data Dependency: The accuracy of the method is highly dependent on the quality and length of the historical data used. If the data set is small or unrepresentative of         future market conditions, it could lead to inaccurate results.

  2. No Forecasting of Future Events: The method doesn't consider changes in market conditions that could occur in the future, such as shifts in volatility, interest rates,        or new market shocks.

  3.Extreme Events or Outliers: Rare events (like the 2008 financial crisis) may or may not be captured depending on the time period of the historical data used. If extreme       events didn’t occur in the period used for historical simulation, they won’t be reflected in the VaR estimate.

