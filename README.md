# IMDB-5000Movie-Score-Profit-Prediction-Model
EDA, Data wrangling and predictive models for imdb movies scores and movie profitabilities using Python 

## Dataset
This project worked on the Kaggle Imdb 5000 Movies Dataset : https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset/data. The dataset includes 4998 movie entires and 28 columns.


## Description
The goal of analysis is to build statistical models for 
1) predicting imdb movies scores,
2) movie profitabilities (using break-even).
Note that this is a practice project, the main focus was on data wrangling and methodological implementation.

## Content
### 1.Exploratory Data Analysis 
### 2.Data Cleaning and Transformation 
- including : variable transformations 
    -  loggross, logbudget,
    -  Recoding categorical variables and get dummies
    -  Creating new variables:  
        - ‘profited’ : binary variable for whether gross profit >= budget (not economically meaningful, just an indicator)
        - ‘director_count’: movie count by director
        - ‘director_meanimdb’ : calculating mean score for movies from the same director

### 3.Prediction models
#### 3.1 Predicting imdb score

- Lasso CV for tuning alpha

- Feature slection 

#### 3.2 Classification
- **3.2.1 Logstic regression classifier**
  
  Confusion matrix:
  
<img width="219" height="178" alt="image" src="https://github.com/user-attachments/assets/3d58b106-4715-4634-b805-229cbf5d6b9a" />

- **3.2.2 Decision tree model**

  Confusion matrix: 
 
 <img width="224" height="177" alt="image" src="https://github.com/user-attachments/assets/18cd5654-6e50-41b2-ada6-dd4e00b5dbb3" />
