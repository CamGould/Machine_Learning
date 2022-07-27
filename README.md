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
This file conatins the [Raw CSV Data](https://github.com/CamGould/Machine_Learning/tree/main/Supplemental) provided by *University of Toronto*
<br>
### Project Outline and Instructions
#### Credit Risk Resampling
In [this notebook](https://github.com/CamGould/Machine_Learning/blob/main/Coding%20Notebooks/%5B1%5DCredit_Risk_Resampling.ipynb), I will use the imbalanced learn library to resample the *Lending Club* data and build and evaluate logistic regression classifiers using the resampled data.
<br>
<br>
The outline of this notebook will be as follows:
<br>
1. Read the CSV into a DataFrame.
2. Split the data into Training and Testing sets.
3. Scale the training and testing data using the StandardScaler from sklearn.preprocessing.
4. Use the provided code to run a Simple Logistic Regression:
    1. Fit the *logistic regression classifier*.
    2. Calculate the *balanced accuracy score*.
    3. Display the *confusion matrix*.
    4. Print the *imbalanced classification report*.
5. Oversample the data using the *Naive Random Oversampler* and *SMOTE algorithms*.
6. Undersample the data using the *Cluster Centroids algorithm*.
7. Over and under sample using a *combination SMOTEENN algorithm*.

For each of the last three points I will:
<br>
1. Train a *logistic regression classifier* from *sklearn.linear_model* using the resampled data.
2. Calculate the *balanced accuracy score* from *sklearn.metrics*.
3. Display the *confusion matrix* from *sklearn.metrics*.
4. Print the *imbalanced classification report* from *imblearn.metrics*.

#### Credit Risk Ensemble

In [this notebook](https://github.com/CamGould/Machine_Learning/blob/main/Coding%20Notebooks/%5B2%5DCredit_Risk_Ensemble.ipynb), I will will train and compare two different ensemble classifiers to predict loan risk and evaluate each model. I will use the [Balanced Random Forest Classifier](https://imbalanced-learn.org/stable/references/generated/imblearn.ensemble.BalancedRandomForestClassifier.html) and the [Easy Ensemble Classifier](https://imbalanced-learn.org/stable/references/generated/imblearn.ensemble.EasyEnsembleClassifier.html). Feel free to refer to the documentation for each of these to read about the models and see examples of the code
<br>
<br>
The outline of this notebook will be as follows:
<br>
1. Read the data into a DataFrame using the provided starter code.
2. Split the data into training and testing sets.
3. Scale the training and testing data using the *StandardScaler* from *sklearn.preprocessing*.

Then for each model I will complete these steps:
1. Train the model using the quarterly data from LendingClub provided in the Resource folder.
2. Calculate the balanced accuracy score from sklearn.metrics.
3. Display the confusion matrix from sklearn.metrics.
4. Generate a classification report using the imbalanced_classification_report from imbalanced learn.
5. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.
