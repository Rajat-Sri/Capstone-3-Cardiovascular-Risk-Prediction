# Capstone-3-Cardiovascular-Risk-Prediction

**Busines problem** - We have been provided dataset with the goal of creating a classification model to predict whether the patient has a 10-year risk of future coronary heart disease (CHD) or not.

**Data Wrangling** -  It is the process of transforming and mapping data from one raw data form into desired format to make it more appropriate and valuable for our analytics. The goal of data wrangling is to assure quality and useful data.

We will perform some basic data cleaning like removing null values and duplicates.

**Data Analysis and Visualization**

**Objective** - We are trying to find how other facorts are influencing the chances of getting affected by coronary heart diseases in next 10 years.

**Analysis Insights**
- Count of people with risk of coronary heart disease in next 10 years is 511 which makes 15% of the total dataset.
- Ratio of men prone to coronary heart disese is higher compared to women.
- Percentage of men who are smokers is comparetevely higher than women.
- There is 4% higher chance of getting infected by coronary diseases if a person is a smoker.
- Quantity of smoking is certainly directly related to coronary heart disese.
- Poor BMI ratio is directly affecting heath of patience.
- It is notable here that patients with high sugar levels are more prone to coronary heart diseases.
- Around 40% of people who have sugar have some type of coronary heart diseases.
- Chance of getting some kind of coronary heart disease increases by 23% if a patient is diabetic.
- Around 50% of patients already suffered heart stroke are affected by colonary hear diseases
- Chance of getting some kind of coronary heart disease increases by 31% if a patient has suffered a heart stroke.
- Normal high side of blood pressure in around 120mm Hg,and we can clearly see patients having blood pressure over this range have got heart stroke.
- Patients who have high blood pressure suffer from hypertension.
- Around 23% of patients have some kind of coronary heart disease who are suffering from hypertension.
- Chance of getting some kind of coronary heart disease increases by 12% if a patient has hypertension.
- Bp medicines are not affective in preventing coronary heart diseases.
- Chance of getting some kind of coronary heart disease increases by 19% if a patient is already taking bp meds.

**Feature Engineering & Data Pre-processing**

- Handling missing values
- Feature manipulation and selection
- Handling outliers
- Categorical Encoding
- Handling imbalance
- Data Transformation
- Data Splitting
- Data Scaling
- Dimentionality Reduction

**ML Model Implementation,cross validation and hyperparameter tuning**
 - Model 1 - Logistic Regression
 - Model 2 - Random Forest
 - Model 3 - XG Boost Classifier

**Conclusion**
- If we want to completely avoid any situations where the patient has heart disease, a high recall is desired. Whereas if we want to avoid treating a patient with no heart diseases a high precision is desired.
- As both evaluation metrics are equally important,we are looking at both F1 score (conveys the balance between the precision and the recall) and False Negatives(recall) for our predictions.
- Both random forest and XG Boost models were performing well,but as random forest model was overfitting data, we have choosen XG Boost classification for our final model building.
