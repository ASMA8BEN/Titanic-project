#Titanic Survival Prediction - Supervised Learning Project

This project served to Build a machine learning model that predicts whether a passenger survived the Titanic disaster based on features such as age, sex, ticket class, and more.

#Project Objective

- Build a classifier to predict survival on the Titanic dataset.
- Apply data preprocessing and feature engineering techniques.
- Train and evaluate multiple machine learning models.
- Optimize the best model using GridSearchCV.
- Generate final predictions for submission.

#Dataset

Data source: [Kaggle Titanic Dataset](https://www.kaggle.com/competitions/titanic/data)

- "train.csv": Training data with features and target ("Survived")
- "test.csv": Test data for final predictions (without labels)

#Features Used

- "Pclass" : Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- "Sex" : Gender
- "Age" : Age of the passenger
- "SibSp" : Number of siblings or spouses aboard
- "Parch" : Number of parents or children aboard
- "Fare" : Ticket fare
- "Embarked" : Port of embarkation (C, Q, S)
- "Title" : Extracted from the passenger’s name (engineered feature)

#Data Exploration
- Summary statistics, missing values
- Visualization of survival rate by gender, class, and age group

#Preprocessing
- Handling missing values (age, fare, embarked)
- Encoding categorical features (sex, embarked, title)
- Feature engineering (title extraction, column cleaning)

#Model Training and Evaluation
- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier
- Evaluation using accuracy, precision, recall, and confusion matrix

#Hyperparameter Tuning
- "GridSearchCV" applied on Random Forest
- Best parameters Random Forest MODEL:
  {'n_estimators': 200, 'max_depth': 8, 'min_samples_split': 2}