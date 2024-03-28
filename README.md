# Predictive Modeling for Credit Card Default Risk Assessment

## [Source Code](https://github.com/saisadhan/Predictive-Modeling-for-Credit-Card-Default-Risk-Assessment/blob/d89abfa035941c498fa4494853613f81137ffd49/Predictive%20Modeling%20for%20Credit%20Card%20Default%20Risk%20Assessment.ipynb)

Welcome to the Predictive Modeling for Credit Card Default Risk Assessment repository. This project aims to leverage supervised machine learning algorithms to predict credit card default, aiding BestCard, a leading credit card company, in enhancing their risk management strategies and minimizing financial losses due to customer defaults.

## Introduction

In this project, we analyze a dataset comprising demographic and financial information for 30,000 account holders. Our objective is to develop predictive models that accurately identify customers at risk of defaulting on their credit card payments. By uncovering patterns and trends associated with defaulting behavior, we enable proactive measures to mitigate risks and optimize customer retention strategies.

### Data Description

- **LIMIT_BAL**: This feature includes both the individual consumer credit and their family (supplementary) credit.
- **Gender**: 1 represents male, and 2 represents female.
- **Education**: 1 indicates graduate school, 2 indicates university, 3 indicates high school, and 4 indicates others.
- **Marital Status**: 1 indicates married, 2 indicates single, and 3 indicates others.
- **Age**: Represents the age of the credit card holder in years.
- **PAY_1 to PAY_6**: These columns represent the payment status of credit card holders for the last six months:
  - **-2**: Indicates no consumption; the credit card holder had no outstanding balance.
  - **-1**: Indicates that the credit card holder paid the full balance.
  - **0**: Indicates that the credit card holder paid the minimum payment but not the full balance.
  - **1**: Indicates that the credit card holder made a payment delay for one month.
  - **2**: Indicates that the credit card holder made a payment delay for two months.
  - ...
  - **8**: Indicates payment delay for eight months.
  - **9**: Indicates payment delay for nine months and above.
- **Amount of bill statement (BILL_AMT1 - BILL_AMT6)**: Represents the amount of bill statement for the last six months.
- **Amount of previous payment (PAY_AMT1 - PAY_AMT6)**: Represents the amount paid for the last six months.
- **Default Payment Next Month**: This column typically represents whether a credit card holder defaulted on their payment in the next month. 
  - **1** indicates that the individual defaulted on their payment.
  - **0** indicates that the individual did not default on their payment.
- **Education_cat**: Likely represents the education level of the cardholders, encoded into categorical values such as graduate school, university, high school, or others.
- **graduate school, high school, others, university**: These columns encode the education levels of cardholders into binary values, indicating whether they belong to specific education categories.

### Data Exploration

#### Key Findings of the Dataset:

- **Number of Samples**: 26,664
- **Number of Columns**: 31
- **Classification of Data Types**: 
  - 11 Categorical
  - 14 Numerical
- **Age of the Customers**: The age of customers ranges from 21 to 79 years.
- **Number of Duplicates & Null Values**: There are 0 duplicates and null values present in the dataset. 

These findings provide a foundational understanding of the dataset, highlighting its size, structure, and integrity, which are crucial for subsequent analysis and model development.

#### visualization of Distribution of Features:
![Image]() 

### Data Cleaning

In this project, we followed a rigorous data cleaning process to ensure the quality and reliability of our dataset. Here's a summary of the steps we took:

- **Handled Missing Values and Duplicates**

- **Dealt with Outliers**

- **Addressed Inconsistencies in Data Formats**

- **Encoded Categorical Variables** - Categorical variables such as SEX, EDUCATION, MARRIAGE, PAY_1 to PAY_6 were encoded to numerical values using appropriate techniques like one-hot encoding or label encoding, enabling our machine learning algorithms to process them effectively.

- **Dropped Irrelevant Columns** -  Columns such as ID, EDUCATION_CAT, graduate school, high school, none, others, and university were identified as irrelevant for our analysis and were dropped to streamline the dataset and enhance model performance.

By meticulously cleaning and preprocessing our data, we ensure that our predictive models are built on a solid foundation, leading to more accurate and reliable results.

## Business Proposal

- **Mitigate Credit Card Default Risk**
- **Drive Sustainable Growth**
- **Leverage ML Expertise**

## Business Outcomes

- **Risk Management Enhancement**
- **Targeted Interventions for High-Risk Customers**
- **Credit Policy Optimization**
- **Customer Retention Strategies**
- **Resource Allocation for Collections**
- **Product and Service Development**
- **Continuous Improvement**

### Model Building

In this phase of the project, I split the data into training and testing sets using an 80:20 ratio. This allowed me to train my models on a subset of the data and evaluate their performance on unseen data.

I employed various predictive machine learning algorithms to build robust models capable of predicting credit card defaults. These algorithms included:

- Decision Tree: A tree-like model where decisions are made based on the features at each node.
  
- Logistic Regression: A regression model used for binary classification tasks, suitable for predicting default probabilities.
  
- Bagging: A meta-algorithm that combines multiple models to improve performance, often used with decision trees.
  
- Boosted Model: A technique that sequentially builds models, each correcting errors of the previous ones, typically used with weak learners.
  
- Random Forest: An ensemble learning method that constructs a multitude of decision trees and merges them to get a more accurate and stable prediction.
  
- Grid Search: A hyperparameter tuning technique that exhaustively searches through a specified parameter grid to optimize model performance.

My goal was to compare the performance of these models and identify the most effective approach for predicting credit card defaults. By leveraging a diverse set of algorithms, I aimed to build robust models that could provide valuable insights for risk management and customer retention strategies.

### Model Evaluation Metrics

For assessing the performance of my predictive models, I focused on two key metrics:

- **Accuracy**: Measures the proportion of correctly predicted instances out of the total instances, providing an overall assessment of correctness.

- **AUC from ROC**: Provides insight into the model's ability to distinguish between positive and negative classes. Higher AUC values indicate stronger predictive ability.

These metrics offered a comprehensive view of my models' performance, guiding decisions on their deployment for risk management strategies.

### Model Accuracy Comparison

![Image]()

### Visualization of ROC Comparison

![Image]()

### Model Deployment Proposal

**Objective:**
Deploy predictive models effectively for credit card default risk assessment, ensuring seamless integration and ongoing optimization.

**Integration Planning:**
- **Define Requirements:** Outline necessary features for deployment, aligning with business objectives.
- **Infrastructure Assessment:** Evaluate existing infrastructure for compatibility and scalability.

**Model Deployment:**
- **Development of API:** Create a robust API for interaction between models and systems.
- **Testing:** Conduct thorough testing to validate functionality and accuracy.

**Monitoring and Maintenance:**
- **Performance Monitoring:** Implement systems for continuous model performance monitoring.
- **Feedback Loop:** Establish mechanisms for user feedback to drive iterative improvements.

**Ongoing Evaluation and Updates:**
- **Regular Reviews:** Schedule periodic reviews to assess model effectiveness.
- **Model Retraining:** Plan regular model retraining for continued relevance and accuracy.

This deployment proposal ensures smooth integration and optimization of predictive models for informed risk management strategies.

### Business Suggestions

To optimize risk management and customer retention efforts, consider:

- **Early Intervention Strategies**: Proactively identify and address potential default risks.
  
- **Customized Communication**: Tailor communication to individual customer needs and preferences.
  
- **Credit Limit Adjustments**: Dynamically adjust credit limits based on risk profiles.
  
- **Financial Literacy Programs**: Offer educational resources for improved financial management.
  
- **Integration with Customer Service**: Incorporate predictive analytics into customer support for personalized assistance.

These suggestions aim to enhance operational efficiency and foster stronger customer relationships.

### Conclusion

Through a comprehensive analysis of the credit card dataset, valuable insights into customer behavior and credit risk have been unveiled. The successful model competition has identified AdaBooster as the leading model, paving the path for innovative risk management strategies.

### Future Prospects
Looking ahead, there are exciting prospects for embracing data-driven decision-making in finance. Opportunities abound for implementing advanced risk management techniques that leverage the power of predictive analytics.

Thank you for your attention and engagement in this endeavor.

**THANK YOU**
