<h1 align="center">A Machine Learning Project Using Imbalenced Classes</h1>
<h2 align="center"> Risky Business </h2>
<h4 align="center"> Created by <em>Cam Gould</em> for the <em>University of Toronto Fintech BootCamp</em> </h4>

<p align="center">
  <img
    src="https://github.com/CamGould/Machine_Learning/blob/main/Supplemental/credit-risk.jpg?raw=true"
  >
</p>

### Background Information
Mortgages, student and auto loans, and debt consolidation are just a few examples of credit and loans that people seek online. Peer-to-peer lending services such as Loans Canada and Mogo let investors loan people money without using a bank. However, because investors always want to mitigate risk, a client has asked that you help them predict credit risk with machine learning techniques.
<br>
<br>
In this assignment, I will build and evaluate several machine learning models to predict *credit risk* using data you'd typically see from peer-to-peer lending services. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I will need to employ different techniques for training and evaluating models with *imbalanced classes*. I will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using ***Resampling*** & ***Ensemble Learning***.
<br>
### Project Files
Use the following links to jump right into the anaylsis notebooks:
<br>
<br>
This notebook contains [Credit Risk Resampling](https://github.com/CamGould/Machine_Learning/blob/main/Coding%20Notebooks/%5B1%5DCredit_Risk_Resampling.ipynb)
<br>
This notebook contains [Credit Risk Ensemble](https://github.com/CamGould/Machine_Learning/blob/main/Coding%20Notebooks/%5B2%5DCredit_Risk_Ensemble.ipynb)
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
