**SyriaTel Customer Churn**

![image1](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/6895f25d-96f8-4ad9-b143-d6256b387c4e)


**Business Problem**

Syriatel is a mobile network provider in Syria. It is one of the only two providers in Syria. The stakeholders would like to reduce money lost by customers who do not stick around for long.

**Business Objective**

The aim of this project is to analyze customer minutes, calls, charge and other variables to predict whether a customer will churn doing business with Syriatel or not.

**Distribution of Customer Churn**

![Pic1](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/920531c9-aa29-465f-9639-82e8165bccf6)

14.49% of the customers would churn the business while 85.51% would not churn.

**Total Day Minutes Vs Churn**
![Pic2](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/f297ee2d-e29d-44a0-bb18-c5ef4cdc8299)

Customers with high number of minutes used during the day are more likely to churn.

**Total Day Charge Vs Churn**
![Pic3](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/9d82ce6a-a1aa-4dfa-9483-5b4abb1a1131)

Customers with a high charge on day time usage are more likely to churn. 

**Customer Service Calls Vs Churn**
![Pic4](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/083b6e85-bdb6-4a5b-b216-4be80fba6426)

Customers who made more customer service calls are more likely to churn.

**Number of Voice Mails Vs Churn**
![Pic5](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/49f78584-80c1-4f61-b189-604fb8d1a121)

Customers with high number of voice mails are less likely to churn.

**Correlation HeatMap of relationship of all variables**
![Pic6](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/474ca558-a572-4c35-a259-9cc739b46c91)


**Model Metrics**
![Pic7](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/7125ba03-1cd2-4a84-b865-a5eeca508f09)

The Decision Tree Classifier has the highest accuracy score and F1 Score, and lowest mean squared error, mean absolute error. Therefore, the Decision Tree Classifier is a good fit for predicting the customer churn.

**Feature Importance**
![Pic8](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/a4376484-9e4a-4578-8e0b-09129a7b0a45)

From the Decision Tree Classifier Feature Importance we can see that total day minutes, total int charge, total intl calls are the most important features for predicting customer churn.Therefore, the company should focus on these features to reduce the customer churn.

**ROC and AUC**

![Pic9](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/0061118c-3160-4c74-a5cd-3d1e8d5c73bb)

![Pic10](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/6c3d983b-4bc1-4ade-96a2-71e2a59a24b1)

![Pic11](https://github.com/BedanNjoroge/SyriaTel_Customer_Churn/assets/118848352/af0f64c9-82a6-41b9-a657-33438abe4082)


The Decision Tree model is performing relatively well with a higher AUC, indicating strong discriminatory power. The KNN model has a lower AUC but is still acceptable. After using XGBoost to increase our model performance the AUC increased a little from 0.890 to 0.897

**Conclusion and Recommendations**

Insights from EDA:
High international calls correlate with lower churn.
High day minutes and charges increase churn.
More customer service calls lead to higher churn.
Customers with more voice mails are less likely to churn.
Recommendations:

Promote international calls.
Lower day charges.
Focus on customer service resolution.
Encourage voice mail usage.
Decision Tree Model:

Highest accuracy and F1 score.
Key features: total day minutes, total intl charge, total intl calls.
Good fit for predicting churn.
XGBoost Improvement:

AUC increased to 0.897.
Accuracy improved to 97.33%.
Outperformed Decision Tree (95.2%).

