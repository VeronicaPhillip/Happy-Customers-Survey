# Happy Customers Survey - Project

The objective of the project was to build a machine learning classifier to predict if a customer is happy or not based on their responses to the survey questions,
identify the questions or features that are most important in predicting  a customer’s happiness and determine whether there is any question that can be removed in 
the next survey. 

# Background and Problem Statement

ACME is one of the fastest growing startups in the logistics and delivery domain. The company works with several partners and makes on-demand delivery to customers. 
During the COVID-19 pandemic, we are facing several different challenges and everyday we are trying to address these challenges.

One of ACME's goals is making their customers happy. As a growing startup, with a global expansion strategy the company has determined that it is necessary to measure 
how happy each customer is. If the company can predict what makes their customers happy or unhappy, then necessary actions can be taken to ensure that customers remain
happy with the service.

Customer feedback is used to determine how happy the customer is with the service and this information is used to improve the company’s operations at all levels in the
organisation.

# Project overview
The project was carried out using the data from the Happiness Survey carried out by the company in 2020. The data consists of 126 rows and 7 columns. One column is the 
target column that indicates whether a customer was happy or not and the other 6 columns represents the responses to the questions asked in the survey. Refer to the data 
dictionary for more details on the information given in each column.

In this project python was used to build predictive models. Classification techniques used to predict the likelihood of a customer being happy or not. We will identify 
the features or questions that are most likely to make customers happy. Multiple models such as Logistic Regression, Decision Trees, Random Forest and ensemble methods 
such as Bagging, and Boosting were used to create models and make predictions using these models. Model performances were evaluated and assessed using accuracy as the 
metric. We aimed to identify models that could achieve accuracy levels above 73%.  

The dataset was cleaned and transformed using feature engineering and split into training (70%) and testing (30%) test sets.

# Prerequisites
To run the code, there were a number of Python libraries that needed to be installed. These are as follows:

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Logistic RegressionCV
* DecisionTree Classifier
* Bagging Classifier
* StandardScaler
* Metrics
* Train_test_split, cross_val_score, GridSearchCV
* Accuracy_score


# Summary/Findings

Summarising the results, we can see that the Decision Tree Model achieved accuracy levels of 73% on the test set and as a result is the best performing model.

The Logistic regression, Decision Tree with Adaboost, Decision Tree with Gradient boosting and Random Forest models all achieved accuracy scores below 73%, with Logistic regression and Random forest performing the worst with test score of 62%.

From the chi squared test results, we can also see that the feature of least importance was X2 followed by X4 (as seen in the Chi squared test). From this we can conclude that in the next survey the Question two (X2) and Question four (X4) could be left off the modelling process as these questions are the least important in predicting the customers happiness in these models.

As the Decision Tree model is the best performing model using accuracy as the metric, this model would be selected over the others and questions X2 and X4 in this case 
would be the least important in determining the customers happiness.




