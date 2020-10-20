# Titanic: Machine learning from disaster(Logistic regression)

## Data

**Dataset:** 
 - The dataset used in the project is obtained from [Kaggle](https://www.kaggle.com).
 - The dataset can be downloaded from [Titanic Dataset](https://www.kaggle.com/c/titanic/data) [Accessed: 9 October, 2020].

**Dataset properties:** 
 - The data has been split into two groups:
   - train.csv
   - test.csv
 - Dataset contains 10 columns in train.csv while test.csv used for prediction does not have the 'Survived' column.
 
| Variable  | Definition | Key |
| ------------- | ------------- | ------------- |
| survival  | Survival  | 0 = No, 1 = Yes|
| pclass  | Ticket class  | 1 = 1st, 2 = 2nd, 3 = 3rd |
| sex  | Sex  |  |
| Age  | Age in years  |  |
| sibsp  |# of siblings / spouses aboard the Titanic  |   |
| parch  | # of parents / children aboard the Titanic |   |
| ticket  | Ticket number  |   |
| fare  | Passenger fare  |  |
| cabin  | Cabin number  |  |
| embarked  | Port of Embarkation  | C = Cherbourg, Q = Queenstown, S = Southampton |

 - **pclass:** A proxy for socio-economic status (SES)
    - 1st = Upper
    - 2nd = Middle
    - 3rd = Lower
 - **age:** Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5
 - **sibsp:** The dataset defines family relations in this way...
     - Sibling = brother, sister, stepbrother, stepsister
     - Spouse = husband, wife (mistresses and fiancés were ignored)
 - **parch:** The dataset defines family relations in this way...
    - Parent = mother, father
    - Child = daughter, son, stepdaughter, stepson
    - Some children travelled only with a nanny, therefore parch=0 for them.

## Files
There are 2 types of files in the repository:
 - Titanic_ligistic_regression.ipynb is the full version of the code used for this predictive analysis
 - readme.md explains the repository

**Result analysis**
 - We built a logistic regression model for prediction
 - Prediction on the given test.csv file resulted a 75.598% accuracy. See here on the [Kaggle Leaderbord](https://www.kaggle.com/c/titanic/leaderboard#score)
 - Splitted test data from train.csv resulted 82.04% accuracy.

**Suggested ways for a better accuracy**
 - More feature engineering such as:
     - grab the name of the passenger, detach dr,mr,mrs and apply them to predict
     - cabin information may have some influnce as it locates the location of the passenger
     - ticket information may have some predictive values worth trying

 **Re-creating the project**
  - In order to perform the analysis step by step please go for the Titanic_logistic_regression.ipynb file.
  - The same analysis can be done in many other ways yet reach the same results. This one is the easiest of the forms possible in my knowledge.
