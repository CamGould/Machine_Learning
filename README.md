<h1 align="center">A Time-Series Analysis Project using Time-Series Models</h1>
<h2 align="center"> A Yen for the Future </h2>
<h4 align="center"> Created by <em>Cam Gould</em> for the <em>University of Toronto Fintech BootCamp</em> </h4>

<p align="center">
  <img
    src="https://github.com/CamGould/Time_Series_Analysis/blob/main/Supplemental/unit-10-readme-photo.png.jpeg?raw=true"
  >
</p>

### Background Information
The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies.
<br>
<br>
In this assignment, I will test multiple time series tools that you have been learned in order to predict future movements in the value of the Canadian dollar versus the Japanese yen.
<br>
### Project Files
Use the following links to jump right into the anaylsis notebooks:
<br>
<br>
This notebook contains [Times Series Forecasting](https://github.com/CamGould/Time_Series_Analysis/blob/main/Coding%20Notebooks/%5B1%5DTime_Series_Forecasting.ipynb)
<br>
This notebook contains [Linear Regression Forecasting](https://github.com/CamGould/Time_Series_Analysis/blob/main/Coding%20Notebooks/%5B2%5DLinear_Regression_Forecasting.ipynb)
<br>
This file conatins the [Raw CSV Data](https://github.com/CamGould/Time_Series_Analysis/blob/main/Raw%20Data/cad_jpy.csv) provided by *University of Toronto*
<br>
### Project Outline and Instructions
#### Time-Series Forecasting
In [this notebook](https://github.com/CamGould/Time_Series_Analysis/blob/main/Coding%20Notebooks/%5B1%5DTime_Series_Forecasting.ipynb), I will load historical CAD-JPY exchange rate data and apply time series analysis and modelling to determine if there is any predictable behaviour between the currencies.
<br>
<br>
The outline of this notebook will be as follows:
<br>
1. Plotting the **"Settle" price** to check for *long or short-term* patterns.
    1. Are there any patterns, long-term and/or short?
2. Decomposition using a **Hodrick-Prescott Filter** (decompose the settle price into *trend and noise*)
    1. Are there any patterns - long or short term?
3. Forecasting returns using an **ARMA model**. 
    1. Based on the p-value, is the model a good fit?
4. Forecasting the *exchange rate price* using an **ARIMA Model**.
    1. What does the model forecast will happen to the Japanese Yen in the near term?
5. Forecasting *volatility* with **GARCH**.
    1. What does the model forecast will happen to volatility in the near term?

#### Linear Regression Forecasting

In [this notebook](https://github.com/CamGould/Time_Series_Analysis/blob/main/Coding%20Notebooks/%5B2%5DLinear_Regression_Forecasting.ipynb), I will build a Scikit-Learn linear regression model to predict CAD/JPY returns with lagged CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).
<br>
<br>
The outline of this notebook will be as follows:
<br>
1. **Data preparation** (creating returns and lagged returns, and splitting the data into training and testing data)
2. *Fitting* a **linear regression model**.
3. Making *predictions* using the **testing data**.
4. **Out-of-sample** performance.
5. **In-sample** performance.
