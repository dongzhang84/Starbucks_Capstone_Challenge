# Starbucks Capstone Challenge

### Introduction:

This is a capstone project of the Udacity data science nanodegree program. This dataset contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

### Dataset

The dataset includes three json files:
 * portfolio.json: containing offer ids and meta data about each offer (duration, type, etc.)
 * profile.json: demographic data for each customer
 * transcript.json: records for transactions, offers received, offers viewed, and offers completed


### Problem Statement

The primary problem I would like to look into is how likely a customer received an offer will complete it. In order to understand this question, I am building a supervised machine learning classification model based on the offer portfolio and demographics information. 

To better understand the data, more questions need to be asked before machine learning modeling. Here, I list five questions I explored:

 * What is the relation between the rate of viewed/completed offer and offer difficulty level?
 * What is the relation between the rate of viewed/completed offer and offer duration?
 * Is there any correlation between offer types and offer completed rate?
 * For individual customers, what are the relations between customer ages, income, membership duration, and offer completed rate?
 * Is customer gender important for final offer completed rate?

The model metrics are given in the session of machine learning modeling.


**Model Metrics**

Supervised classification models were built and most accuracy model was selected. The main metrics for model performance are

- Precision
- Recall
- Weighted F1 score
- ROC AUC score


### Conclusions

I delivered a series of analytic results, and built a model to predict if an offer will be completed by a customer. 

**Analytic Results**

The data shows that there is no customer completed the received offers if
- The offer difficulty level is 0.
- The offer duration is less than 5.
- The offer type is informational.

Also I found that younger people, people with lower salaries, relatively new members, or men are less likely to complete offers. To increase revenue, Starbucks need to focus more on data where shows higher offer completed rate. 

**Predictor Model**

The machine learning model gives a predictor for individual customer to complete an offer. The difficulty level, income, age, channel and offer types tare among the topic importance for the model. The model accuracy (F1 score) is $\sim$0.8. So far the offer completed rate is 0.46, the predictor with much higher probability to target individual customer helps Starbucks to significantly increase customers' offer completed rate.


### Blog

Medium blog: https://dongzhanghz.medium.com/starbucks-capstone-challenge-1736efb047b6









