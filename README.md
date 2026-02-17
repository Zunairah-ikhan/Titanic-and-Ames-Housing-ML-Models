# ML Models for the Titanic and Ames Housing datasets
## Dataset Descriptions
>I. Titanic Dataset  
>[https://www.kaggle.com/c/titanic/data](https://www.kaggle.com/c/titanic/data)  
>The RMS Titanic was a British ocean liner, the largest ship of its time, that sank on 15th of April, 1912 after colliding with an iceberg during her maiden voyage. The infamous sinking of the "unsinkable" resulted in the death of approximately 1502 of its 2224 passengers. Though there was some element of luck involved in surviving, some groups seemed more likely to survive than others. In this notebook, we will build a model to predict just that, answering the question, "what sort of people were more likely to survive?” We will be using the actual passenger data, albeit with all its shortcomings, as its a classic dataset, especially suitable for classification tasks.

>II. Ames House Prices Dataset  
>[https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)  
>A dataset for predicting house prices based on features like size, location, and amenities. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, this competition challenges you to predict the final price of each home. The Ames Housing dataset was compiled by Dean De Cock for use in data science education. It's an incredible alternative for data scientists looking for a modernized and expanded version of the often cited Boston Housing dataset.


## Tasks performed in the Jupyter notebook for both datasets:

### 1.  Data Acquisition & Initial Exploration
*  Loading the dataset using pandas
*  Displaying basic information and analysing: `info()`, `describe()`, and `head()`
*  Identifying missing values and deciding on a strategy for handling them
### 2.  Data Preparation & Preprocessing
*  Splitting the data into features **`X`** and target `y`
*  Using `sklearn.model_selection.train_test_split` to create training and test sets
*  For the Titanic dataset, using stratified sampling based on the Survived column
*  For the Housing dataset, using random sampling
### 3.  Building a `scikit-learn` Processing Pipeline
*  Imputating missing values (median for numeric & mode for categorical)
*  Encoding categorical variables using `OneHotEncoder`
*  Scaling of numeric features using `StandardScaler`
*  Feature selection using `SelectKBest` with `f_regression` and `f_classif`
*  Training a logistic regression model for the Titanic dataset
*  Training a linear regression model for the Housing dataset
### 4.  Model Evaluation & Comparison
*  Classification metrics: Accuracy, Precision, Recall, F1-score
*  Regression  metrics: RMSE and R² score
*  Compare performance with a baseline model:
*  Majority class for classification
*  Mean prediction for regression
### 5.  Feature Engineering
*  Creating at least two new features for each dataset:
   *  Titanic: `FamilySize` and `Title` extracted from `Name`
   *  Housing: `AgeOfHouse` and `TotalSquareFootage`
*  Retraining pipeline with the new features and evaluating if performance improves

### References
1.  DagsHub. *Baseline models*. [https://dagshub.com/glossary/baseline-models/](https://dagshub.com/glossary/baseline-models/)
2.  Geeks for Geeks. *Machine learning*. [https://www.geeksforgeeks.org/machine-learning/machine-learning/](https://www.geeksforgeeks.org/machine-learning/machine-learning/)
3.  Géron, A. (2017). *Hands-on machine learning with Scikit-Learn and TensorFlow* (1st ed.). O’Reilly.
4.  May, M. (2023). *Tackling the Ames housing dataset*. Medium [https://medium.com/@mskmay66/tackling-ames-housing-dataset/](https://medium.com/@mskmay66/tackling-the-ames-housing-dataset-c63e7947908a)
5.  Singh, R. (2024). *Introduction to machine learning*. Medium. [https://medium.com/introduction-to-machine-learning/](https://medium.com/@RobuRishabh/introduction-to-machine-learning-555b0f1b62f5)
6.  Thacker, N. (June, 2025). *Data preprocessing and exploratory analysis of the titanic dataset: a comprehensive machine learning approach*. [https://niyatithacker.github.io/Sinking-into-Stats/](https://niyatithacker.github.io/Sinking-into-Stats/)
7.  Wikipedia. *Machine learning*. [https://en.wikipedia.org/wiki/Machine_learning](https://en.wikipedia.org/wiki/Machine_learning)
