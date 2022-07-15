# FlatironPhase3Project

Peter Burton

Flatiron Data Science Bootcamp Phase 3

Data from Kaggle: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset

Presentation: https://docs.google.com/presentation/d/1pHAk258q4okdgybgRiEnrwEDiacMCAOBAelH7GV52PU/edit?usp=sharing

## Busines Problem

My task is to work as a  Telcom consultant to predict customer churn. By providing Telcom providers a way to correctly predict customer churn, we are enabling them to to begin customer retention or other long term programs aimed at reducing areas that cause customer loss. 

Cost of customer aquistion is high, but telcom customers tend to often stay with one provider for a long time period, so being abble to correctly analyze and predict customer churn will enable a provider to institute customer outreach and retention, or create incentives and discounts that can prevent churn at a much lower cost then aquiring a new customer. 

## Dataset

We are working from a dataset of 3333 Telcom customers, with profile infrmation inluding 20 differnt predictors that are based roughly around customer use patterns, and the churn column.The churn is our target variable variable, with a typical churn rate of about 14%,  and the other 20 predictor classes will help us model and correctly classify churn scenarios. 

## Model

Our Classification model is attempting to find the best possible model that predicts along the Recall metric. Because customer retention efforts can be relatively low cost, we do not mind having a certain amount of false positives, instead we want to focus on correctly identofying the highest possible number of customers that will churn. 


Our modeling process takes a look at different classifered and uses different features. Starting with a dummy model that predicts base on most common result, and moving forwards with gridsearchs on models such as Decision Trees, Gradient Boosting, K Nearest Neighbors, and Random forest. 


## Results

After itterating through different models, and tuning the perametors of the grid seachers, we improved our model drastically. The Dummy model had a recall score of 0%, initial logistic regression model with just 3 features had a recall score of 67%, and  our final and most accurate model was the Gradient Boost model after tuning paramters and introducing SMOTE oversampling to the dataset. Althought the Gradient Boost model recall score score hovered around 90% on the training data, it showed some signs of being overfit and only scored around 70% on the test data. 


## Conclusion

Based on our model, the telcom customer retention program should be focused on the three initial areas we identified in the intial data exploration phase: State data, daily charge data, and customer service call data. In addition, Customers that use the international plan, as well as customers that have high voicemail usage are at elevated churn risk. 

## Action Plan

-Identify Key factors in high churn states such as competition and create customer loyalty and retention programs in those states that create a competitive edge vs other competitors in those markets

-Find ways to reduce sticker shock and daily use discounts that can target high churn risk customers that have high daily charges

-Identify systemic issues that cause multiple customer service calls and ways to increase customer sastisfaction

-Identify if cost or other reasons are causing churn with international plan customers and create a more cost effective international plan

-Make voicemail set-tup and use more seamless and and create systems that prevents spam calls 
