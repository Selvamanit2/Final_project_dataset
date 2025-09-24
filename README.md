# ***1. Project Overview***

*We are trying to predict the global air pollution levels using different models. We used features like Country,	City,CO AQI Value,Ozone AQI Value,NO2 AQI Value. We tested many models and tuned them to check which one gives the best result.*

##***2. Dataset Details***

***Features used:***

- Country
- City
- CO AQI Value
- Ozone AQI Value
- NO2 AQI Value
- PM2.5 AQI Value

***Target:***
- AQI Category

***Preprocessing:***

- Label encoding for categorical columns.
- StandardScaler used for scaling.
- Split data into train and test (80%-20%),

## ***3. Model Results***
| Model              | Accuracy | F1 Score   |
| -----------------  | -------- | ------
| LogisticRegression |	0.6143	|   0.69
|	Decision Tree	     |  0.7226	|   0.73
|K-Nearest Neighbors |	0.6732	|   0.73
|XGBoost Classifier	 | 0.6956	  |  0.73
|SupportVectorMachine|	0.6445	|   0.74

>Best model → Decision Tree (72.26%)

###  ***4. GridSearchCV – Hyperparameter Tuning***
**Decision Tree:**

Best parameter

'criterion': ['gini', 'entropy']

'max_depth': [3, 5, 10, None]

Best score: *0.722063*

**XGBoost**

Best parameter

'n_estimators': [50, 100, 200]

'max_depth': [3, 5, 7]

'learning_rate': [0.01, 0.1, 0.2]

Best score:*0.707349*

# ***5.Real-World Benefits:***
- **Health Protection –**
Helps people avoid exposure to polluted air by giving early warnings, reducing risks like asthma, lung disease, and heart problems.

- **Government & Policy Support –**
 Assists pollution control boards and city authorities in making data-driven decisions (e.g., traffic control, industrial regulation).

- **Smart City Integration –**
Can be connected with IoT sensors for real-time air quality monitoring in smart cities.

- **Environmental Awareness –** Spreads awareness about pollution and motivates people to adopt eco-friendly practices.

- **Mobile & Web Applications –** Can be used in apps or websites to give daily air quality updates and safety recommendations to the public.

###  ***6. Insights:***
- Model is Accuracy was 0.7226
- using tuning score was increse in XGBoost model
- more feature are add maybe model perfomance increse

