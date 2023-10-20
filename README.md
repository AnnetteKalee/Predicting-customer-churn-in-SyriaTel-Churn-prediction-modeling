# Predicting-customer-churn-in-SyriaTel-Churn-prediction-modeling
# Churn prediction modeling

**Author**: [Annette Kalekye](annette.kalekye@student.moringaschool.com)

## Project Overview

This project aims to predict customer churn and identify patterns indicating loss of customers for SyriaTel a telecommunications company,aiming to retain customers to reduce revenue and acquistion costs loss and increase customer lifetime. 

### Business Problem

There is increased competition in the telecommunications industry and most companies experience a very high churn rate which in turn leads to loss of revenue and acquisition costs. Retaining existing customers is the most cost-effective method to keep business running compared to acquiring new ones. Targeting SyriaTel's business needs,this project aims to optimize customer retention strategies by analyzing predictable patterns, benefiting the company's financial sustainability.


### The Data

The data used in this project is from SyriaTel telecommunications company: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset


## Methods

This project applies data analysis, feature engineering, encoding and three models to come up with the most optimal predictive model fro customer churn and determine the most important features in predicting churn.

## Modeling

1. **Baseline Model** Metrics and interpretation

Accuracy: 0.85 85% of the predictions made by the baseline model were correct.

Precision: 0.67 Out of the instances predicted as positive, only 67% were correct.

Recall: 0.06 Only 6% of the actual positive instances were correctly predicted

F1 Score: 0.11 The harmonic mean of precision and recall, indicating a balance between precision and recall. A low F1 score suggests poor performance in terms of both false positives and false negatives.

ROC AUC: 0.53 A value of 0.53 indicates the model's performance is not much better than random chance.

3. **Complex Model**: Random forest metrics and interpretation 

 Accuracy: 0.97 97% of the predictions made by the models were correct.

 Precision: 0.97 Out of the instances predicted as positive, 97% were correct.

 Recall: 0.83 83% of the actual positive instances were correctly predicted.

 F1 Score: 0.89 the harmonic mean of precision and recall is 0.89, indicating a good balance between precision and recall.

 ROC AUC: 0.91 ROC AUC is 0.91, suggesting a strong ability to distinguish between positive and negative classes.

4. **Hyperparameter tuning and optimization** metrics and interpretation

Accuracy: 0.97 97% of the predictions made by the models were correct.

Precision: 0.97 Out of the instances predicted as positive, 97% were correct.

Recall: 0.83 83% of the actual positive instances were correctly predicted.

F1 Score: 0.89 the harmonic mean of precision and recall is 0.89, indicating a good balance between precision and recall.

ROC AUC: 0.91 ROC AUC is 0.91, suggesting a strong ability to distinguish between positive and negative classes.


+ The Baseline Model has poor recall (6%),it fails to identify most of the actual positive instances. Its overall performance is weak compared to the Complex Model and Tuned Model.

+ Both the Complex Model and Tuned Model have significantly improved performance. They have high accuracy, precision, and recall. The F1 score and ROC AUC are also high, indicating a good balance between precision and recall.

+ The Complex Model and Tuned Model have similar metrics, indicating that the hyperparameter tuning did not result in a significant improvement. However, both models are performing exceptionally well compared to the Baseline Model.

5. Most important data features.

+ we visualized feature importance to understand which features are most influential in predicting customer churn, see below:

   
   ![image](https://github.com/AnnetteKalee/Predicting-customer-churn-in-SyriaTel-Churn-prediction-modeling/assets/136931914/6d342465-5ba0-4219-978f-8faf0b955f7d)
## Conclusion

The model predictions were useful in this contexts:

+ **High Usage Patterns**: High usage may correlate with loyal customers less likely to churn.
+ **Short Contract Lengths**:  Short-term customers may be more prone to churn compared to those with long-term contracts.
+ **Customers with Customer Service Interactions**:  High numbers of customer service calls could indicate customer dissatisfaction and potential churn.
+ **Specific Service Subscriptions**: The model may excel in predicting churn for customers with these specific services.
+ **Customer Segmentation**: Demographic factors like age, location, or income can influence churn patterns. If specific segments have distinct churn behavior, the model could be useful in predicting churn within these segments.


## Recommendations

This analysis leads to these recommendations for SyriaTel:

+ **Targeted Marketing Campaigns**: Focus marketing efforts on customers identified as high-risk for churn. 
+ **Customer Service Improvements**: Investigate the reasons behind customer service calls. If a significant portion of churned customers made multiple service calls, consider enhancing customer support, providing additional training to customer service representatives, or improving online self-service resources.
+ **Product/Service Enhancements**: Identify features or services that are popular among long-term customers. Consider expanding or promoting those features to attract new customers and retain existing ones.
+ **Customer Feedback Loop**: Establish a feedback mechanism to understand the reasons behind customer churn. Surveys, feedback forms, or follow-up emails can provide valuable insights into customer dissatisfaction, helping the company address specific pain points.
### Limitations

+ **Low Churn Rate**: If the dataset has a low churn rate,the model might struggle to accurately predict churn due to class imbalance. It might be biased towards predicting the majority class (non-churn) and overlook churn instances.
+ **Change of Customer Behavior**: Customer behavior is not rigid it changes over time. Patterns that were relevant in the past might not be indicative of churn in the future. The model might struggle to adapt to evolving customer preferences and behaviors.
+ **Unseen Patterns**: If the model was not trained on specific patterns (e.g., new services or marketing strategies), it might not accurately predict churn in situations it has not encountered before.
+ **Limited Features**: If crucial features related to customer satisfaction, like survey results or social media sentiment, are not included, the   model might lack vital information to make accurate predictions.
+ **Data Quality**: Inaccurate or incomplete data can lead to misinformed predictions. Missing or erroneous data points might affect the model's performance negatively.

