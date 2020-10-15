# pandas_homework

## Quantitative Analysis

After conducting quantitative analysis on the different portfolios, which included calculating and plotting the *cumulative* returns for each investment strategy, only two portfolios outperformed the S&P 500: Algo 1 and Berkshire Hathaway. Additionally, it should be noted that Algo 1 was the top performer and while Algo 2 did not "beat" the market, it did outpace the other portfolios under consideration. 

## Risk

### Box Plots

Any investment decision would be inadequate if it did not include a risk analysis of the different options on the table. Part of this analysis typically would include a measure of the variability of the different investment options. Box plots are helpful in accomplishing this analysis as they allow investors to visualize the distribution, central value and variability of each performance. As we can see from the graph above, Algo 2 has the smallest smallest distribution, or spread, between its maximum and minimum values, indicating that it is a relatively safe choice in comparison to the other options.

### Standard Deviations

Another measure of risk for an investment strategy would be standard deviations, which is a measure of the amount of variation or dispersion of a set of values, which in this case would be the portfolio's daily returns. A low standard deviation indicates that the values *tend* to be close to the mean while a high standard deviation indicates that the values *tend* to spread out over a wider range. Therefore, a low standard deviation would be indicative of a less risky investment strategy when compared to a strategy with a higher standard deviation. 

In the case of this analysis, it is helpful to compare a portfolios riskiness to that of the market. After comparing the standard deviations of the different portfolios to that of the S&P 500 you can see that there are several options that are less risky: Soros Fund Management, Paulson & Co. Inc., Algo 1 and Algo 2. Additionally, Tiger Global Management and Berkshire Hathaway Inc. would be considered more risky under this analysis. These results remain true if the standard deviations were to be annualized.

## Rolling Statistics

### Correlation to General Market Risk

In addition to calculating risk for a single point in time it is helpful to measure risk as it moves through time and fluctuates upwards or downwards. In order to do this we can use rolling, or moving, statistics which will create a series of standard deviations for different subsets of the full data set. In this case, we will be using a 21 day look back window to quantify the change in risk. After plotting the rolling standard deviations for each of the portfolios, we can see that most do see an increase in their own risk as the market's risk increase, although this correlation is not perfect. For example, Berkshire Hathaway routinely has a higher standard deviation than the market during general times of increased volatility while most of the rest of the portfolios enjoy a less pronounced upswing in dispersion. Additionally, Tiger Global Management LLC's risk appears to have little correlation to the market. In times of low volatility for the market and other portfolios, Tiger Global Management periodically suffers from large increases to its own risk. 

### Correlation Table

While the above visualization is helpful, it might be more useful to quantify the correlation between the different portfolios and the general stock market (S&P 500). After creating a correlation table using Python, we can see that Algo 2 most closely mimics the S&P with a relatively high coefficient of correlation (a 0.858764 coefficient with 1.0 being perfectly correlated) in comparison to the other portfolios.

### Berkshire Hathaway Beta

Beta is a useful way to measure the riskiness of a stock or an investment by comparing it to the broader market. By definition, the market (i.e. the S&P 500) is 1.0 and a beta above that threshold is more volatile than the market but offers greater potential returns. A beta below 1.0 indicates an investment that is less risky than the overall market but offers potentially lower returns. As we can see from the graphical representation above, Berkshire Hathaway has, *generally*, a lower beta than the market meaning that it is a stable investment.  

## Sharpe Ratios

The sharpe ratio is a useful piece of information for investors as it is used to convey the return of an investment compared to its risk. The ratio is the average return earned in excess of the risk-free rate per unit of volatility, which would be a measure of the price fluctuations of the portfolios in question. 

After calculating the sharpe ratios for each of the portfolios and plotting them next to each other, we can see that the Algo 1 portfolio was the top performer and even beat out the S&P 500. While Algo 2 was outpaced by Berkshire Hathaway and the market, it still carried a higher risk ratio in comparison to the remaining portfolios. 

## Custom Portfolio

After constructing a custom portfolio made up of Google, Twitter and JP Morgan stock, I conducted a similar analysis of those made above. In terms of cumulative returns, this custom portfolio performed very well, outpacing the market and each portfolio except for Algo 1. However, this custom portfolio did have a higher standard deviation as compared to the S&P 500 and experienced higher bouts of volatility during times of uncertainly, similar to Berkshire Hathaway.

While this is concerning, it is also noteworthy to point out that the custom portfolio had a very similar sharpe ratio to that of the S&P 500 (0.713602 vs 0.718630) and enjoyed a higher sharpe ratio compared to every portfolio except for Algo 1 and had a beta below 1.0 indicating that it is a relatively stable investment strategy. 