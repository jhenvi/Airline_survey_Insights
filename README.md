# Airline Customer Satisfaction Survey Results

 
# Customer Satisfaction Analysis and Prediction

This notebook is to showcases:
- Basics of data science (data cleaning, encoding, feature engineering, and model training)
- Predicting Customer Satisfaction based on the customer satisfaction survey, with customer feedback on their experience 
  with the airline 
 ###### Data Source: others:Kaggle https://seaborn.pydata.org/index.html#
 
 1. Import data files, pandas, matplotlib, seaborn, numpy, spicy & Skelearn
 2. Clean and transform dataset Survey Results
 - The plot shows a distribution of around 55%:45% between neutral/dissatisfied
 passengers and satisfied passengers respectively. 
 - The data is balanced and does not require any special treatment/resampling
 3. Graphical presentation of customer satisfaction survey responses 
 ###### Gender Analysis Survey Results: 
 - shows gender-wise distribution of dissatisfied and satisfied customers are quite the same. 
 - For both male and female passengers, the number of dissatisfied customers is not higher than the satisfied customers.
###### Customer Type Analysis Survey Results
- The number of loyal customers is higher than the non-loyal. Among loyal passengers, the ratio of satisfied and dissatidfied ones is 49:51.
###### Age Analysis Survey Results
- Age 7-38 and Age 61-79 ranges, quotient of dissatisfied passengers is higher compared to satisfied passengers. 
- Age 39-60 range, quotient of satisfied passengers is higher compared to dissatisfied passengers.
######  Type of Travel, Class, Flight Distance Survey Results:
- Business travel in business class category, the number of satisfied passengers are higher than longer flight distance. 
- Other combinations, there is almost equal distribution of satisfied and dissatisfied passengers.
######  Survey Results, online Boarding, departure/Arrival time Convenience grouped by Class: 
- Eco Plus class, Departure/Arrival time has negative responses with high number of dissatisfied passengers. 
- Other combinations, there is higher level of satisfaction.
###### Survey Results, departure delay, arrival delay grouped by type of travel: 
- Personal travel (specially Eco Plus and Eco), has higher number of dissatisfied passengers when arrival delay in minutes is high. 
- By minute comparison, all combinations have higher number of dissatisfied passengers compared to satisfied passengers.
##### Survey Results, baggage handling, gate location grouped by class: 
- Business class, it is observed that all gate locations have higher number of dissatisfied passengers when baggage handling is not done perfectly well (rating <= 4). 
- Passengers remained dissatisfied, when the gate location is 1 and for Eco, when the gate location is 2, even when the baggages are handled in a mediocre way (rating in range 2.0 - 4.0).
##### Survey Results, inflight entertainment, inflight wi-fi service grouped by Class: 
- Economy Plus passengers are mostly satisfied without in-flight wi-fi service (rating 0) and medium level of in-flight entertainment (rating 2 - 4). 
- Business class passengers, with only a highest level of in-flight entertainment (rating 5), customer is satisfied. 
- Economy passengers, with high level of in-flight entertainment (rating 3 - 5) and high wi-fi service availability (rating 5), customer is satisfied.

### 4 Label encoding of categorical variables
- Outliers Detection and Removal, calcuations of IQR
- Remove outliers from dataset
### 5. Top 10 Features Selection through Chi-Square

### 6. Feature Importance using Wrapper Method

### 7. Feature Permutation Importance
- https://eli5.readthedocs.io/en/latest/autodocs/sklearn.html
- https://machinelearningmastery.com/how-to-fix-futurewarning-messages-in-scikit-learn/

### 8. Building Models
#### Model-1: Logistic Regression penalized with Elastic Net (L1 penalty = 50%, L2 penalty = 50%)
- 11 out of the 12 features in the survey results (except:Inflight_entertainment), have p-value < 0.05.
- A p-value less than 0.05 (typically ≤ 0.05) is statistically significant. 
- It indicates strong evidence against the null hypothesis, as there is less than a 5% probability the null is correct (and the results are random).
- These features have hight impact towards the target variable. A pseudo R-square value (McFadden's Pseudo R-Squared Value) of 0.55 represents an excellent fit.

### Model-2: Naive Bayes Classifier

### Model-3: K-Nearest Neighbor Classifier

### Model-4: Decision Tree Classifier

### Model-5: Neural Network (Multilayer Perceptron)

### Model-6: Random Forest

### Model-7: Extreme Gradient Boosting

### Model-8: Adaptive Gradient Boosting

### 9. Decision Region Plotting for Different Models¶

### 10. Model Comparison