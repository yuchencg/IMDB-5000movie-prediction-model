# IMDB--5000Movie-DataAnalysis--PredictionModel
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
<img width="548" height="307" alt="output1" src="https://github.com/user-attachments/assets/cba2f559-3355-466e-b03e-0f03ad751222" />

- Feature slection 
  
<img width="858" height="649" alt="output2" src="https://github.com/user-attachments/assets/c229083b-3a3f-48aa-9370-3dd4aeece1d4" />

- ### 3.2 Classifing 
- **3.2.1 Logstic regression classifier**
  
  Confusion matrix:
  
<img width="509" height="437" alt="output3" src="https://github.com/user-attachments/assets/e295abc5-7ae9-4ff8-ba74-dbea6fdcae52" />

- **3.2.2 Decision tree model**
  
 <img width="1696" height="1175" alt="output4" src="https://github.com/user-attachments/assets/00456aa1-6046-4a41-a0bf-8bfd52f66934" />

  Confusion matrix:
  
  <img width="509" height="437" alt="output5" src="https://github.com/user-attachments/assets/0099deb1-e3ed-466e-b23d-3341c184d4be" />
