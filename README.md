# ML Models for the Titanic and Ames Housing datasets

>I. Titanic Dataset
>[https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data)
>The RMS Titanic was a British ocean liner, the largets ship of its time, that sank on 15th of April, 1912 after colliding with an iceberg during her maiden voyage. The infamous sinking of the "unsinkable" is often considered as one of the most deadly sinkings resulting in the death of approximately 1502 of its 2224 passengers. Though there was some element of luck involved in surviving, some groups seemed more likely to survive than others. So in this notebook, we will build a model to predict just that, answering the question, "what sorts of people were more likely to survive?” We will be using the actual passenger data, albeit with all its shortcomings, as its a classic dataset especially suitable for classification tasks.

>II. Ames House Prices Dataset
>[https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
>A dataset for predicting house prices based on features like size, location, and amenities. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home. The Ames Housing dataset was compiled by Dean De Cock for use in data science education. It's an incredible alternative for data scientists looking for a modernized and expanded version of the often cited Boston Housing dataset.


Tasks performed in the Jupyter notebook for both datasets:
1.  Data Acquisition and Initial Exploration
    *  Load the dataset using pandas
    *  Display basic information: `info()`, `describe()`, and `head()` to analyze
    *  Identify missing values and decide on a strategy for handling them
2.  Data Preparation and Preprocessing
    *  Split the data into features (X) and target (y)
    *  Use `sklearn.model_selection.train_test_split` to create training and test sets
    *  For the Titanic dataset, use stratified sampling based on the Survived columnExplain why this is appropriate.
    *  For the House Prices dataset, use random sampling. Justify your choice.
3.  Building a Processing Pipeline
Create a scikit-learn pipeline that includes:
• Display basic information: info(), describe(), and head().
• Imputation of missing values (using median for numeric, mode for categorical).
• Encoding of categorical variables (use OneHotEncoder).
• Scaling of numeric features (use StandardScaler).
• Feature selection using SelectKBest with f_regression/f_classif.
Train a linear regression model (House Prices) and a logistic regression
model(Titanic) within the pipeline.
4.  Task 4. Model Evaluation and Comparison (15 points)
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
