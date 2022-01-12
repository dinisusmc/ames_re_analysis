# Ames Houseing Market

## The goal of this project was to; 

### 1.) Upload Ames real estate data.
### 2.) Clean the raw data.
### 3.) Encode categorical features and fill missing values.
### 4.) Exploratory Data Analysis on the data to investigate features.
### 5.) Create a predictive model based on any theories.
### 6.) Submit your predictions to the kaggle competition.
### 7.) Present your findings to stakeholders.

## As seen in my the ./code/AmesMarketAnalysis.ipynb I will break down my approach to this situation;

### 1.) After loading in the data, I checked it for features with missing values and  which features are categorical.
### 2.) I decided to exclude any features missing more than 350 values because using Kneighbors to predict possible values would be skewed missing close to 20% of the data for that feature.
### 3.) I then created a pipeline with a column transformer to one hot encode the remaining categorical features, and impute any missing values.
### 4.) I used a mask to filter the DataFrame and return a list of only features that correlated greater than or less than what ever percentages you input.
### 5.) Using the correlated DataFrame I set up multiple models in line so you can run them all after changing the filter inputs.
### 6.) Results are dependent on the training data used to fit the model, my best submission was using gs2 or gs3 pipeline for predictions.

## Based on these findings I made 3 reccomendations to help add value to a property in Ames;

### 1.) Improve the Quality of the house.
### 2.) Increase the livable area in the house.
### 3.) Add a garage if feasible.

## Code NoteBook;
### ./project2/code/AmesMarketAnalysis.ipynb

## Data Dictionary Available;
### https://www.kaggle.com/c/dsir-907-project-2/data

## Kaggle Submission is availabe at; 
### https://www.kaggle.com/c/dsir-907-project-2/submissions?group=selected&page=1&pageSize=100;

## The training data used for modelling;
### https://www.kaggle.com/c/dsir-907-project-2/data?select=train.csv

## The test data predicted on (excluding the 'SalePrice' column);
### https://www.kaggle.com/c/dsir-907-project-2/data?select=test.csv