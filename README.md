# Quantitative-Analysis-of-Financial-Markets

### Projecting Singapore’s GDP by Industry Sectors to assess the impact of Covid-19. 

#### Background: 
Singapore’s economy had been ravaged by the Covid-19 pandemic. No sector in Singapore’s economy is left unscathed. Until, the pandemic, Singapore’s economic trajectory had always been upwards, hence our group is interested in finding out how much damage Covid-19 has done and how Singapore Government has responded to support different sectors. In this project we utilized statistical models to predict the growth of Singapore’s sector GDP without the effect of Covid-19, compared against the actual GDP and estimated the impact on different sectors.
#### Methodology:

a)	Data Source:
We sourced the GDP data for the period between 1975 to 2020 (first 2 quarters) from the Singapore Department of Statistics (https://www.singstat.gov.sg/), and for the purpose of this project, we selected the 4 biggest sectors which contributed the most to Singapore’s GDP for further analysis, namely: Manufacturing, Wholesale & Retail Trade, Business Services and Finance & Insurance. 


b)	Handling of Data:
For the data to be fitted into VAR and ARIMA model, we have performed the following steps:
1.	Visualize the time series
2.	Test stationarity of time series
3.	Lognormalised the data
4.	Decompose the time series
5.	Perform first differencing to the data
6.	Test stationarity of time series
7.	Test for causality amongst the time series
8.	Test for cointegration

c)	Model Fitting:
For the purpose of this project, VAR is a suitable model because it not only takes the input of its own time series, but also that of the other related time series of other industries in the modelling of its behaviour. ARIMA model is the alternative choice when VAR model’s conditions are not satisfied.

For VAR model, we fitted the data in with increasing AR order, and selected the optimal model parameter based on the lowest AIC criterion. However, we have noticed that the P values of coefficients of Finance & Insurance sector is not within significance level (> 0.05), thus we used the ARIMA model instead. For ARIMA Model, we used ACF and PACF to determine the model parameters. To test the robustness of the model, we performed various statistical tests, such as the Durbin Watson test, ACF and PACF tests, Back Test etc. 


#### Findings and Conclusion:
Our project shows that Covid-19 had the greatest impact on the sectors of Manufacturing as well as Wholesale & Retail Trade. This was probably due to the nature of Manufacturing and Wholesale & Retail Trade sectors, which require employees to be physically present at their workplace.

The Business Services sector also experienced a downturn in GDP growth, but the impact of covid-19, was not so great compared to Manufacturing and Wholesale & Retail Trade sectors. We think that is so because employees from Business Services sector can continue to work from home and remain productive.

The Finance & Insurance sector experienced growth despite the adverse impact of Covid-19. This is probably because it is less dependent on Singapore’s local market and more on the global economy. Employees in this sector could also work from home without much disruption.





