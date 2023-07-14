# Capstone-3-Cardiovascular-Risk-Prediction

## Problem Statement: 
In this project on cardiovascular risk prediction, our main goal was to create a classification model to predict whether a patient has a 10-year risk of future coronary heart disease (CHD) or not. We worked with a dataset, which provided information on various patient attributes that could potentially be risk factors for cardiovascular disease.

## Data Wrangling:
To prepare the data for analysis, we performed data wrangling tasks such as handling missing values and duplicate values. We replaced missing values with median values since the percentage of missing data was less than 10% and it would not significantly affect the data skewness. We also corrected the data types of variables to ensure consistency.

## Exploratory Data Analysis (EDA):
We conducted an exploratory analysis of the dataset to gain insights and understand the relationships between variables. We examined the distributions of risk factors like glucose levels, cholesterol levels, body mass index (BMI), and heart rate. This helped us understand the data and identify patterns.

## Feature Engineering: 
For feature engineering, we used correlation coefficient analysis to select the most important features. We found that variables like smoking and cigarettes per day were highly correlated, so we removed smoking as it could be derived from the cigarettes per day variable. We also created a new variable called "hypertension" to address the high correlation between systolic and diastolic blood pressure. Additionally, we removed irrelevant or highly correlated features from the dataset.

## Handling Imbalanced Data,Data Scaling and Data Splitting: 
To address the imbalance in the dataset, where only around 15% of patients had coronary heart disease, we used oversampling techniques like SMOTE (Synthetic Minority Oversampling Technique) to create synthetic data points for the minority class. We also used the Standard Scaler method to scale the data, ensuring that all features had a mean close to 0 and a standard deviation of approximately 1. And finally we splitted the data into a training set (80%) and a testing set (20%) to evaluate the performance of our models.

## Model Implementation: 
We experimented with different machine learning algorithms to build our predictive models. This included algorithms such as Logistic Regression, Random Forest, and XG Boost Classification. These models were trained on the training data and used to make predictions on the testing data.

## Hyperparameter Tuning: 
Each machine learning algorithm has various hyperparameters that control its behavior. We used techniques like GridSearchCV and random search to find the optimal combination of hyperparameter values for each model. This involved trying different values and evaluating the model's performance using appropriate evaluation metrics.

## Evaluation Metrics:
When evaluating the models, we considered evaluation metrics that were appropriate for imbalanced datasets, such as the F1 score, which balances precision and recall. We selected the XG Boost Classification model as the final prediction model due to its highest F1 score and lower overfitting compared to other models.

## Final Model Selection:
Based on the evaluation metrics and considering factors like model performance, interpretability, and generalization ability, we selected the XG Boost Classification model as our final prediction model. This model demonstrated the best overall performance in terms of the chosen evaluation metrics.

## Model Explainability: 
We analyzed the importance of different features in the XG Boost model to understand their contribution to the predictions. This was done using techniques like permutation importance or SHAP values, which provide insights into which features are most influential in determining the risk of CHD.

## Conclusion:
In conclusion, the project aimed to predict the risk of coronary heart disease in patients using machine learning techniques. By effectively handling missing values, conducting exploratory analysis, performing feature engineering, addressing class imbalance, and selecting appropriate evaluation metrics, we were able to build a reliable prediction model. The selected XG Boost Classification model showed promising results and provided insights into the important risk factors for CHD.
