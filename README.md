
# Customer Churn Prediction 
![Image Alt Text](https://github.com/mercytegekson/Phase3Project/blob/main/customerchurnlogo.JPG)

# Customer Churn Prediction

![SyriaTel Company](https://github.com/mercytegekson/Phase3Project/blob/main/bigml_59c28831336c6604c800002a.csv)


## Problem statement
In the telecommunications industry, customer churn poses a significant challenge to service providers, impacting revenue streams and hindering long-term sustainability. For Syria Tel, the need to proactively identify and address factors contributing to customer churn has never been more pressing. The problem at hand is twofold: the lack of a predictive model for customer churn and a limited understanding of the key drivers that influence customer decisions to terminate their services.
The project's aim is to:
•	Uncover meaningful patterns associated with customer churn, enabling targeted preventive measures to retain customers.
•	Create Machine Learning based predictive models that can show likelihood of a customer leaving the services of SyriaTel Company.


## PROJECT OVERVIEW 
The project focuses on the creation of a machine-learning project for  customer churn prediction for SyriaTel company.

## BUSINESS UNDERSTANDING
Customer Churn is one of the most important and challenging problems for businesses such as Credit Card companies, cable service providers, SASS and telecommunication companies worldwide.
Customer churn refers to customers who have stopped using the services of the company.
Customer churn can be used to define customers who:
Have completely stopped interacting or unsubscribed from a brand, or
Customers who have reduced how often they interact with your brand.


## Components

* **Jupyter Notebook**
The [Jupyter Notebook](https://github.com/mercytegekson/Phase3Project/blob/main/index.ipynb)is our key deliverable and contains details of our approach and methodology, data cleaning, exploratory data analysis and model building and validation.

I recommend using [nbviewer](https://nbviewer.jupyter.org/) to view the Jupyter Notebook.

* **Presentation**
The [presentation](https://) gives a high-level overview of our approach, findings and recommendations for non-technical stakeholders. It is aimed to be between 5 and 10 minutes long.

* **Data**

The dataset can be found in the file *"bigml_59c28831336c6604c800002a.csv"* in the Data folder, in this repository. It was originally provided in the following [repository](https://github.com/mercytegekson/Phase3Project/blob/main/bigml_59c28831336c6604c800002a.csv).

## Technologies/ Packages

* Python version: 3.6.9
* Matplotlib version: 3.1.3
* Seaborn version: 0.9.0
* Pandas version: 0.25.1
* Numpy version: 1.16.5
* Scikit-learn version: 0.21.2  

## To get started

1. Clone this repository - [guidance](https://help.github.com/articles/cloning-a-repository/).
2. Dataset can be found in the file"bigml_59c28831336c6604c800002a.csv".
3. Check requirements in Technologies section above and download libraries if necessary.

## 1. Data Wrangling
Here we will work on data cleaning, handling missing values, data transformation, handling duplicates, data reshaping and other processes to ensure that we have a clean, structured, and suitable format for analysis and modeling

## 2. Exploratory Data Analysis (EDA)
Here we will explore the different features of the dataset to gain a better understanding of the data. We will use data vizualization to uncover trends and patterns. We will use Feature Engineering to create new features from existing ones and perform One-Hot Encoding on categorical variables that we will require for analysis.
Strong predictors of churn include "customer service calls", "international_plan" and "total_charges"


## 3.Baseline model:Logistic Regression Model.
The model exhibits strong predictive performance for the majority class ("False") with high precision (88%), recall (96%), and F1-Score (92%). However, it faces challenges in accurately predicting instances of the minority class ("True"), reflected in lower precision (48%), recall (21%), and F1-Score (29%). This indicates potential difficulties in correctly identifying customers who are likely to churn.

## 4. KNN Model
### KNN Results
The KNN model achieves an accuracy of 87.89%, indicating its overall ability to correctly predict outcomes. In terms of precision, the model demonstrates a satisfactory ability to accurately identify customers who will churn, with a precision of 68%. However, the recall is relatively lower at 31%, suggesting that the model might not capture all instances of actual churn. The F1-score, a balance of precision and recall, is at 43%. The classification report shows that the model performs better in identifying non-churn instances ("False") than churn instances ("True").

### Tuned Model
The final logistic regression model, tuned with the best hyperparameters identified through grid search, achieved an accuracy of approximately 74.82% on the test set. While the final logistic regression model has a lower overall accuracy compared to the baseline logistic regression and the KNN models, it demonstrates improved performance in correctly identifying instances of the minority class ("True"). The F1-score for the "True" class is higher in the final logistic regression model, indicating better balance between precision and recall for churn instances.


## Conclusions
These insights suggest that certain customer behaviors and plan types are strong predictors of churn. Strong predictors of churn include "customer service calls", "international_plan" and "total_charges". Therefore, the segment of customers with international plans, higher total charges, and more customer service calls are at higher risk of churn. A higher number of international calls is associated with a lower likelihood of churn. The column "state_numeric" also plays a role, but the impact might depend on the specific states. Although this model is reliable, it should be used in conjunction with other domain information for more precise prediction of customer churn.













    

