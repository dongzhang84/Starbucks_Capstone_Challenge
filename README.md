# Starbucks Capstone Challenge

### 1. Motivation:

This is a capstone project of the Udacity data science nanodegree program. This dataset contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

**Problem Statement**

The primary problem I would like to look into is how likely a customer received an offer will complete it. In order to achive this goal, I am building a supervised machine learning classification model based on the offer portfolio and demographics information. 

Before working on the modeling, more questions need to be asked to better understand the data. Here, I list five questions I explored:

 * What is the relation between the offer viewed/completed rate and offer difficulty level?
 * What is the relation between the offer viewed/completed rate and offer duration?
 * Is there any correlation between offer types and offer completed rate?
 * For individual customers, what are the relations between customer age, income, membership duration, and offer completed rate?
 * Is customer gender important for offer completed rate?


**Model Metrics**

Supervised classification models were built and most accuracy model was selected. The main metrics for model performance are

- Precision
- Recall
- Weighted F1 score
- ROC AUC score



### Files in the Repo

The dataset in the data folder includes three json files:
 * portfolio.json: containing offer ids and meta data about each offer (duration, type, etc.)
 * profile.json: demographic data for each customer
 * transcript.json: records for transactions, offers received, offers viewed, and offers completed

The code is in this [jupyter notebook](https://github.com/dongzhang84/Starbucks_Capstone_Challenge/blob/master/Starbucks_Capstone_notebook.ipynb).


### Libraries 

This project used Python 3.8.2 with its update-to-date libraries, including:

    numpy
    pandas
    datetime
    matplotlib
    seaborn
    sklearn
    lightgbm
    xgboost




### Conclusions

I delivered a series of data analytic results, and built a machine learning classification model to predict if an offer will be completed by individual customers. 

**Analytic Results**

The data shows that there is no customer completed the received offers if
- The offer difficulty level is 0.
- The offer duration is less than 5.
- The offer type is informational.

Also I found that younger people, people with lower salaries, relatively new members, or men are less likely to complete offers. To increase the revenue, Starbucks needs to focus more on offers featured with higher completed rate. 

**Predictor Model**

The machine learning model gives a predictor for individual customer to complete an offer. The difficulty level, income, age, channel and offer type are among the topic importance for the model. The model accuracy (F1 score) is ~ 0.8. So far the offer completed rate is 0.46, the predictor with much higher probability to target individual customer helps Starbucks to significantly increase customers' offer completed rate.


### Acknowledgements

I thank Udacity and Starbucks to provide the simulated dataset.


### Blog

Medium blog: https://dongzhanghz.medium.com/starbucks-capstone-challenge-1736efb047b6









