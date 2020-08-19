# predicting-credit-card-approval

## Introduction
As manually analysing credit card approval requests are error-prone, time-consuming as well as banks gets lots of requests in which many gets rejects due to numerous reasons such a low income levels. This task has been automated by Machine learning model. 

The dataset for this project has been taken from http://archive.ics.uci.edu/ml/datasets/credit+approval from UCI machine learning repository.
### Steps followed in the project
1. The dataset has been imported. The features in the dataset are anonymized by the contributor of dataset.
2. An attempt to find most important features of a credit card application is made. Exploratory data analysis on the dataset is done.
3. Missing values in the dataset has been handled( replaced with NaN).
4. Missing values are imputed using mean imputation strategy for features containing numerical values.
5. Missing values in other columns are replaced by the most frequent values in respective feature.
6. Data is preprocessed -  Non-numeric data is converted to numeric using label encoding technique, data is splitted into training & test sets, feature values are scaled to a uniform range & un-neccesary features are dropped from the dataset.
8. Logistic Regression model is fitted & trained on the set.
9. Predictions are made & model performance i.e. classification accuracy is evaluated as well as confusion matrix.
10. Model performance is improved using GridSearchCV from sklearn.model_selection to tune hyperparameters.
11. Best achieved score of the model & respective best paramters are stored.


# Instructions to run the code
1. Make a virtual environment
```
python3 -m venv env
```
Activate the virtual environment
```
source env/bin/activate # This command is for linux 
```

2. clone the repository :
```
git clone https://github.com/divya661/predicting-credit-card-approval.git
```
Or

Download the zip folder & unzip the folder downloaded

Install the requirements by running the command in terminal:
pip install -r requirements.txt
Open the jupyter notebook and run the file 'notebook.ipynb' in directory `predicting-credit-card-approval`
