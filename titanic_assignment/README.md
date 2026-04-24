# Titanic Survival Prediction - Assignment 2 
 
## Overview 
This project performs data cleaning, feature engineering, and feature selection on the Titanic dataset. 
 
## Data Cleaning Decisions 
- Age (19%% missing): Imputed with median by title 
- Embarked (0.2%% missing): Filled with mode 'S' 
- Cabin (77%% missing): Created Has_Cabin indicator and extracted Deck 
 
## Features Engineered 
- FamilySize = SibSp + Parch + 1 
- IsAlone = 1 if FamilySize == 1 else 0 
- FarePerPerson = Fare / FamilySize 
- Title extracted from Name 
- AgeGroup: Child, Teen, Adult, Senior, Elderly 
- Deck extracted from Cabin 
 
## How to Run 
1. Install dependencies: pip install -r requirements.txt 
2. Launch Jupyter: jupyter notebook 
3. Open notebooks/Titanic_Feature_Engineering.ipynb 
 
## Dependencies 
- pandas, numpy, matplotlib, seaborn, scikit-learn, jupyter 
