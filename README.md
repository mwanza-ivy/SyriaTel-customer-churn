# SyriaTel-Customer-Churn-Analysis
### ![image](https://github.com/mwanza00/SyriaTel-customer-churn/assets/137791910/037db45c-3bdd-4cde-bb76-b36e2c0501d1)
# Business Case
A telecommunication company called SyriaTel has enlisted data scientists to create a model that predicts when the customers are leaving their business. The data scientist is expected to build an accurate model and report features that may be an indicator that the customer will be more likely to leave.
# Overview
This project focuses on analyzing customer churn using classification models. The goal of this project is to provide valuable insights to SyriaTel, a telecommunications company regarding factors that influence the rate at which customers stop doing business with the company over a given period of time and to make data-driven recommendations on how to reduce the amount of money lost because of customers who don't stick around very long
# Project Goal
The primary goal of this project is to perform a comprehensive analysis of the SyriaTel customer churn data, using classification models. This analysis aims to provide valuable insights into the factors that influence customer churn and make data-driven recommendations for the telecom business and other stakeholders.
# Stakeholders
1. The intended audience for this project includes:

2. Shareholders: Individuals looking to enhance the value of their investments through informed decision-making regarding long-term growth and sustainability.

3. Management: Company leaders and agents seeking data-driven insights to ensure their clients stay in business with them in the long run.

4. Marketing team: Professionals in this department seek to maintain increased customer acquisition, engagement, and delivery of tailored promotions.

5. Customer Support Team: The customer care team works to resolve issues quickly and effectively while also raising customer satisfaction levels.

6. Customers: These are the final consumers who demand trustworthy and reasonably priced telecommunications services.
# Key Questions
1. Which plans are customers satisfied with?
2. Which factors lead to service discontinuation?
3. How can SyraTel retain customers?
# Dataset
We used data sourced from SyriaTel Customer Churn Dataset CSV. The data represents customers with information on different variables. Total data used was from 3333 customers. The dataset has a target variable that indicates whether a customer has churned (1 for "yes" and 0 for "no"). Key variables in oour dataset include: International plan(yes/no), Voicemail plan(yes/no), Number of calls, Number of service calls and Daily charge.
# Data Preparation
1. Exploratory Data Analysis
2. Removed corelated columns
3. Applied SMOTE to remove imbalance
# Visualiations

People with international plans are way more likely to churn. Perhaps other companies are offering more competitive pricing.
![image](https://github.com/mwanza00/SyriaTel-customer-churn/assets/137791910/36cbd72c-a88b-4626-ae25-a77ff85bffa6)

Minutes spent on the phone during the day are correlated with customers leaving the service
### ![image](https://github.com/mwanza00/SyriaTel-customer-churn/assets/137791910/e62b00df-6744-470f-8329-3686fa9c2698)

More than 3 customer service calls from a customer suggest that they are on the brink of leaving
### ![image](https://github.com/mwanza00/SyriaTel-customer-churn/assets/137791910/8acc94ca-f0e1-43ce-b9ff-7690e2d1ae0a)

# Final Model
Best Model: XGBClassifier
Best Score (AUC): 0.9095239466280581
### ![image](https://github.com/mwanza00/SyriaTel-customer-churn/assets/137791910/beb7aec7-e60e-498e-b1f0-3bed75541786)
# Conclusions
Based on the accuracy and ROC curve comparisons, we can decide that the Extreme Gradient Boosting model is the best model to deploy for the churn prediction task. It has the highest accuracy and largest area under the ROC curve (AUC). Additionally,the XGBClassifier model is more practical and suitable when it comes to other factors, such as model interpretability and business requirements.
In practice, it's important to validate the chosen model on new, unseen data to ensure its generalization performance. It's also essential to monitor the model's performance over time and retrain it if necessary, as customer behavior may change.
# Recommendations
1. Increase the quality of customer service to reduce the amount of times called, especially focusing on customers who call repeatedly.
2. Provide better plans for those who use more minutes like decreasing charge rate after hitting a cap of 240 call minutes instead of a flat rate per minutes.
3. Give out some rewards or benefits for customers for their account length over time to promote customer loyalty.
4. Implement customer retention strategies around key predictors like providing added benefits and incentives for customers with an international plan.
