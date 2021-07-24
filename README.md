** Challenge_4**
In this Challenge, I assume the role of a quantitative analyst for a FinTech investing platform. This platform aims to offer clients a one-stop online investment solution for their retirement portfolios that’s both inexpensive and high quality. (Think about Wealthfront (Links to an external site.) or Betterment (Links to an external site.)). To keep the costs low, the firm uses algorithms to build each client's portfolio. The algorithms choose from various investment styles and options.

I have been tasked with evaluating four new investment options for inclusion in the client portfolios. Legendary fund and hedge-fund managers run all four selections. 
**What You're Creating**
I produced a Jupyter notebook that contains your data preparation, analysis, and visualizations for key risk and return metrics. I used text and comments to document my findings and answer the question prompts in the instructions. 

Specifically, this file contains the following:

1.single DataFrame imported from a CSV file that has a DateTimeIndex.

2.risk analysis of the assets that the DataFrame contains vs. the S&P 500. This analysis should include risk-return metrics, including the daily returns,           standard deviation, Sharpe ratio, and beta.

3.evaluation of each asset that uses rolling statistics to track the risk-reward behavior over time.


Download the following files to help you get started:

Module 4 Challenge files

Instructions
For this Challenge assignment, I imported a CSV file and prepared the daily returns DataFrame for analysis. I perform a quantitative analysis that includes the following:

1.Performance

2.Volatility

3.Risk

4.Risk-return profile

5.Portfolio diversification

**Import the Data**
First, I read a CSV file of data into a Pandas DataFrame. This file contains data about portfolios with net asset value (NAV) pricing from four whale investors. The file also contains data about the S&P 500 index, which will serve as the benchmark for your analysis.


**Analyze the Performance**
I Analyze the data to determine if any of the portfolios outperform the broader stock market, which the S&P 500 represents. To do so, I performed the following steps:

1. I used the default Pandas plot function to visualize the daily return data of the four fund portfolios and the S&P 500. 

2. I used the Pandas cumprod function to calculate the cumulative returns for the four fund portfolios and the S&P 500.
 
3. I used the default Pandas plot to visualize the cumulative return values for the four funds and the S&P 500 over time. 


**Analyze the Volatility**
Analyzing the volatility of each of the four fund portfolios and of the S&P 500 Index by using box plots. I completed the following steps:

1.I used the Pandas plot function and the kind="box" parameter to visualize the daily return data for each of the four portfolios and for the S&P 500 in a box     plot. 

2.I used the Pandas drop function to create a new DataFrame that contains the data for just the four fund portfolios by dropping the S&P 500 column. I Visualized   the daily return data for just the four fund portfolios by using another box plot. 

**Analyze the Risk**
 I evaluated the risk profile of each portfolio by using the standard deviation and the beta. I completed the following steps:

1.I used the Pandas std function to calculate the standard deviation for each of the four portfolios and for the S&P 500. 

2.I Calculated the annualized standard deviation for each of the four portfolios and for the S&P 500. I multiplied the standard deviation by the square root of     the number of trading days (252)

3.I used the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of the four fund portfolios and of the S&P 500 index. 

4. I set the daily returns DataFrame and a 21-day rolling window to plot the rolling standard deviations of only the four fund portfolios. 


**Analyze the Risk-Return Profile**
To determine the overall risk of an asset or portfolio, quantitative analysts and investment managers consider not only its risk metrics but also its risk-return profile. After all, if you have two portfolios that each offer a 10% return but one has less risk, you’d probably invest in the smaller-risk portfolio. For this reason, I needed to consider the Sharpe ratios for each portfolio. I completed the following steps:

1.I used the daily return DataFrame to calculate the annualized average return data for the four fund portfolios and for the S&P 500. Use 252 for the number of     trading days. 

2.I calculated the Sharpe ratios for the four fund portfolios and for the S&P 500. To do that, I divide the annualized average return by the annualized standard   deviation for each. 

3.I visualized the Sharpe ratios for the four funds and for the S&P 500 in a bar chart. 


**Diversify the Portfolio**
I evaluated how the portfolios react relative to the broader market. Based on my analysis so far, I choose two portfolios that you’re most likely to recommend as investment options. I completed the following step:

I used the Pandas var function to calculate the variance of the S&P 500 by using a 60-day rolling window. 
I completed the following steps for each of the portfolios I chose:

1.I used the 60-day rolling window, the daily return data, and the S&P 500 returns, to calculate the covariance. 

2.I calculated the beta of the portfolio. To do that, divide the covariance of the portfolio by the variance of the S&P 500.

3.I used the Pandas mean function to calculate the average value of the 60-day rolling beta of the portfolio.

4.I ploted the 60-day rolling beta. Be sure to include the title parameter, and adjust the figure size if necessary.

After completing all of these steps I Finshed the assignment and comitted it to git hub. I then turned the assignment in.


