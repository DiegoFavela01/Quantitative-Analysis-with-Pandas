# Quantitative-Analysis-with-Pandas
## Challenge 4 - University of Berkeley Financial Technology Boot Camp 
This code involves a quantitative analysis of daily returns of four whale investors' portfolios and the S&P 500 index. The analysis includes the following components:
The analysis includes the following components:

- Performance
- Volatility
- Risk
- Risk-return profile
- Portfolio diversification
### Part 1: Importing the Data
To begin the analysis, the whale_navs.csv file was read into a Pandas DataFrame. A DateTimeIndex was created for the DataFrame and the head of the DataFrame was reviewed. Then, a daily returns DataFrame was created using the Pandas pct_change function and dropna on the NAV prices of the four portfolios and the closing price of the S&P 500 Index.

### Part 2: Analyzing the Performance
The data was analyzed to determine if any of the portfolios outperformed the S&P 500. This was done by visualizing the daily return data of the four fund portfolios and the S&P 500 using the default Pandas plot function. The cumulative returns for the four fund portfolios and the S&P 500 were calculated using the Pandas cumprod function and visualized using the default Pandas plot function.

### Part 3: Analyzing the Volatility
The volatility of each of the four fund portfolios and of the S&P 500 Index was analyzed by using box plots. Daily return data was visualized for each of the four portfolios and for the S&P 500 using the Pandas plot function with kind="box" parameter. A new DataFrame was created containing the data for just the four fund portfolios by dropping the S&P 500 column. Daily return data was visualized for just the four fund portfolios using another box plot.

### Part 4: Analyzing the Risk
The risk profile of each portfolio was evaluated by using the standard deviation and the beta. The Pandas std function was used to calculate the standard deviation for each of the four portfolios and for the S&P 500. The annualized standard deviation was calculated for each of the four portfolios and for the S&P 500. The daily returns DataFrame and a 21-day rolling window were used to plot the rolling standard deviations of the four fund portfolios and of the S&P 500 index. The daily returns DataFrame and a 21-day rolling window were used to plot the rolling standard deviations of only the four fund portfolios.

### Part 5: Analyzing the Risk-Return Profile
The Sharpe ratios for each portfolio were calculated to determine the overall risk of an asset or portfolio. The daily return DataFrame was used to calculate the annualized average return data for the four fund portfolios and for the S&P 500. The Sharpe ratios were calculated for the four fund portfolios and for the S&P 500. The Sharpe ratios were visualized for the four funds and for the S&P 500 in a bar chart.

### Part 6: Diversifying the Portfolio
To evaluate how the portfolios react relative to the broader market, the variance of the S&P 500 was calculated using a 60-day rolling window. Then, for each of the two portfolios chosen, the covariance and beta were calculated using the 60-day rolling window, the daily return data, and the S&P 500 returns. The average value of the 60-day rolling beta of the portfolio was calculated and plotted.

## Libraries and Dependencies
This code uses the following libraries:

- Pandas
- Pathlib
- Numpy
- %Matplotlib
####  To install these libraries
```bash
!pip install pandas
!pip install pathlib
!pip install numpy
```
###  Running the Code
To run the code, open a Jupyter Notebook or JupyterLab session and run each cell of the code sequentially. Make sure that the necessary CSV file (whale_nav.csv) are in the same directory as the Jupyter Notebook file.
