# ML Models for the Titanic and Ames Housing datasets

>I. Titanic Dataset
[https://www.kaggle.com/c/titanic/data](ttps://www.kaggle.com/c/titanic/data)
classic dataset for predicting survival
on the Titanic. Suitable for classification tasks. The sinking of the Titanic is one of the
most infamous shipwrecks in history. On April 15, 1912, during her maiden voyage, the
widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg.
Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the
death of 1502 out of 2224 passengers and crew. While there was some element of luck
involved in surviving, it seems some groups of people were more likely to survive than
others.Using this dataset, you asked to build a predictive model that answers the
question: “what sorts of people were more likely to survive?” using passenger data (i.e.,
name, age, gender, socio-economic class, etc).

>II. Ames House Prices Dataset
[https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
A dataset for predicting house prices
based on features like size, location, and amenities. With 79 explanatory variables
describing (almost) every aspect of residential homes in Ames, Iowa, this competition
challenges you to predict the final price of each home. The Ames Housing dataset was
compiled by Dean De Cock for use in data science education. It's an incredible
alternative for data scientists looking for a modernized and expanded version of the
often cited Boston Housing dataset.
Complete the following tasks in a Jupyter notebookfor both datasets.
Task 1. Data Acquisition and Initial Exploration (10 points)
• Load the dataset using pandas.
• Display basic information: info(), describe(), and head().
• Identify missing values and decide on a strategy for handling them (with
justification).
Task 2. Data Preparation and Preprocessing (15 points)
• Split the data into features (X) and target (y).
• Use sklearn.model_selection.train_test_split to create training and test sets.
• For the Titanic dataset, use stratified sampling based on the Survived column.
Explain why this is appropriate.
• For the House Prices dataset, use random sampling. Justify your choice.
Task 3. Building a Processing Pipeline (20 points)
Create a scikit-learn pipeline that includes:
• Display basic information: info(), describe(), and head().
• Imputation of missing values (using median for numeric, mode for categorical).
• Encoding of categorical variables (use OneHotEncoder).
• Scaling of numeric features (use StandardScaler).
• Feature selection using SelectKBest with f_regression/f_classif.
Train a linear regression model (House Prices) and a logistic regression
model(Titanic) within the pipeline.
COEN_COSC_ITAP_3411_202620
Special Topics 1 - Machine Learning
by Dr. Anwar M. Mirza
Assignment 1
Date: February 01, 2026
Due: February 14, 2025, Mid-Night
Page 3 of 3
Task 4. Model Evaluation and Comparison (15 points)
• Load the dataset using pandas.
• Evaluate the model using appropriate metrics:
o Regression: RMSE and R² score
Classification: Accuracy, Precision, Recall, F1-score
• Compare performance with a baseline model (e.g., mean prediction for regression,
majority class for classification).
Task 5. Feature Engineering (10 points)
Create at least two new features for each dataset:
• Titanic: e.g., FamilySize, Title extracted from Name
• House Prices: e.g., AgeOfHouse, TotalBathrooms
Retrain your pipeline with the new features and evaluate if performance improves.
