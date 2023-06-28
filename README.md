# Classification-Project-on-Customer-Churn
Project Title: Predicting Customer Churn: Uncovering Key Indicators and Retention Strategies

Introduction

Customer churn, also known as customer attrition or customer turnover, refers to the percentage of customers who cease using a company's product or service within a given timeframe. Understanding and predicting customer churn is crucial for organizations as it directly impacts their profitability and growth. By identifying the factors that contribute to churn, businesses can develop effective retention strategies to mitigate this problem.

In this project, we will analyze a dataset containing various customer attributes such as gender, age, partner status, internet service provider, contract term, and payment method, among others. We aim to explore the relationship between these attributes and the likelihood of customer churn. By conducting a thorough analysis, we can uncover key indicators of churn and identify patterns that indicate a higher propensity for customers to leave the organization.

Objectives

1.Build a classification model to predict customer churn and assess the likelihood of a customer leaving the organization.

2.Identify key indicators or factors that contribute to customer churn.

3.Formulate effective retention strategies based on the identified indicators to mitigate customer attrition.

Hypothesis

Null Hypothesis: There is no significant relationship between the various customer attributes and the likelihood of customer churn.

Alternate Hypothesis: There is a significant relationship between the various customer attributes and the likelihood of customer churn.



Questions

1.What are the significant factors that influence customer churn?

2.Can we accurately predict customer churn based on available customer data?

3.How can we use the identified indicators to develop effective retention strategies?

4.Which customer segments are more likely to churn?

5.How can the organization leverage payment methods, contract terms, and billing preferences to reduce churn?

Data Collection and Preparation

The data was colleceted from three separate channels. That is from SQL database, onedrive and Azubi git-hub repository. The data was then concatenated into a single dataset. The data was cleaned for consistency and completeness. 

Observations from previewing the data set

There were some missing values in some columns.
The columns customer ID and gender were dropped because they had no significance in the analysis.
Some columns had false, no , true, yes values. false and true values were replaced with no and yes values.

Machine Learning Modelling

Onehotencoding was performed on categorical columns. The data was then split into test and 
train. Then missing values in numerical columns was imputed using the simple imputer method.
SMOTE was applied to balance the train data set. The balanced features and target variable were 
then concatenated into a single DataFrame. The following models; KNeighboursClassifier,
GradientBoostingClassifier, AdaBoostClassifier and RandomForestClassifier were created and 
used to train the data. The following metrics were then employed; accuracy, precision, recall, f1 
score and f2 score. To achieve maximum performance, hyperparameter tuning was employed.
The f1 score metric was used to select the best models as follows:
Model Name F1_Score
GradientBoostingClassifier 0.643312
RandomForestClassifier 0.632836
AdaBoostClassifier 0.621387
KNeighborsClassifier 0.550376




Conclusion and Recommendations

Based on the analysis of the graph, it is evident that customer churn is influenced significantly by 
two key factors: tenure and monthly charges. Tenure has been identified as the highest contributor 
to customer churn, indicating that customers with shorter contract terms, particularly those on a 
month-to-month basis, are more likely to terminate their contracts compared to those with longerterm commitments. Furthermore, monthly charges also play a significant role, suggesting that 
customers with higher monthly charges are more prone to churn.
Additionally, the graph highlights that the electronic check payment method has the highest churn 
rate among the different payment methods. This implies that customers using electronic checks as 
their payment method are more likely to churn compared to those using alternative payment 
options.
Based on the findings, it is crucial for the company to focus on addressing the issues related to 
customer churn, particularly in relation to tenure, monthly charges, and payment methods. Here 
are some recommendations to mitigate churn:


Offer Flexible Payment Methods: Provide customers with a variety of payment options such as electronic check, mailed check, bank transfer (automatic), and credit card (automatic). This allows customers to choose the payment method that suits them best, increasing convenience and reducing the likelihood of churn due to payment-related issues.

Incentivize Long-Term Contracts: Encourage customers to sign up for longer contract terms (e.g., one year or two years) by offering benefits such as discounted rates, additional services, or loyalty rewards. Longer contracts provide stability and commitment, making customers less likely to churn.

Personalize Billing Preferences: Allow customers to choose their billing preferences, such as paperless billing or traditional paper billing. Some customers prefer the convenience of electronic billing, while others may prefer physical copies. By accommodating individual preferences, the organization can enhance customer satisfaction and reduce churn.

Analyze Customer Behavior and Preferences: Utilize customer data to analyze patterns and identify correlations between payment methods, contract terms, billing preferences, and churn. Look for trends or insights that indicate specific combinations of these factors that are associated with higher or lower churn rates. This analysis can help the organization tailor their retention strategies and target specific customer segments.

Proactive Retention Strategies: Implement proactive measures to prevent churn. For example, identify customers who are approaching the end of their contract term and offer them incentives to renew or upgrade their services. Additionally, provide personalized offers or promotions to customers who have shown signs of potential churn based on their payment patterns or billing preferences.

Improve Customer Support: Ensure that customer support services are readily available to address any payment-related concerns or billing inquiries. Prompt and effective resolution of customer issues can help build trust and loyalty, reducing the likelihood of churn.

Continuous Monitoring and Optimization: Regularly monitor and analyze customer feedback, behavior, and churn rates associated with different payment methods, contract terms, and billing preferences. Continuously optimize and refine the organization's strategies based on the insights gained, aiming to align offerings with customer preferences and needs.

By leveraging payment methods, contract terms, and billing preferences in these ways, the organization can enhance customer satisfaction, increase retention rates, and ultimately reduce churn.
