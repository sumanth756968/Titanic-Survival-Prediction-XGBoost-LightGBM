# Titanic Survival Prediction Using XGBoost and LightGBM

## 📌 Project Overview

This project predicts passenger survival using the **Titanic dataset** and compares two powerful gradient boosting algorithms: **XGBoost** and **LightGBM**.

The project includes Exploratory Data Analysis (EDA), data preprocessing, model training, performance evaluation, hyperparameter tuning, model comparison, and final prediction generation.

## 🎯 Objectives

* Explore the Titanic dataset.
* Analyze missing values and feature distributions.
* Perform data preprocessing.
* Encode categorical variables.
* Train XGBoost and LightGBM classification models.
* Evaluate both models using multiple performance metrics.
* Tune LightGBM hyperparameters using GridSearchCV.
* Compare XGBoost and LightGBM performance.
* Generate Titanic survival predictions.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost
* LightGBM
* Jupyter Notebook

## 📂 Dataset

The project uses two datasets:

* `Titanic_train.csv`
* `Titanic_test.csv`

The target variable is:

`Survived`

## 🔄 Project Workflow

1. Import required libraries
2. Load training and testing datasets
3. Explore dataset structure
4. Check missing values
5. Perform Exploratory Data Analysis
6. Visualize numerical and categorical features
7. Remove unnecessary columns
8. Handle missing values
9. Encode categorical variables
10. Split training data into training and validation sets
11. Train LightGBM model
12. Train XGBoost model
13. Evaluate both models
14. Perform LightGBM hyperparameter tuning
15. Compare model performance
16. Predict survival on the test dataset
17. Generate `submission.csv`

## 🔍 Exploratory Data Analysis

The project uses:

* Histograms
* Boxplots
* Survival count plots
* Gender vs Survival analysis
* Passenger Class vs Survival analysis

These visualizations help identify patterns and relationships within the Titanic dataset.

## 🧹 Data Preprocessing

The following preprocessing steps are performed:

* Remove `PassengerId`, `Name`, `Ticket`, and `Cabin`
* Fill missing `Age` values using the median
* Fill missing `Fare` values using the median
* Fill missing `Embarked` values using the mode
* Encode `Sex` and `Embarked` using LabelEncoder
* Split the data into training and validation sets

## 🤖 Machine Learning Models

### LightGBM

LightGBM is used as a gradient boosting classification algorithm for predicting passenger survival.

### XGBoost

XGBoost is another gradient boosting algorithm used to build a classification model and compare its performance with LightGBM.

## 📊 Evaluation Metrics

Both models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score

A comparison table and bar chart are also created to visualize the performance of the two models.

## ⚙️ Hyperparameter Tuning

GridSearchCV is used to tune the LightGBM model.

The parameters tested include:

* `n_estimators`
* `learning_rate`
* `max_depth`

Three-fold cross-validation is used to identify the best parameter combination.

## 📄 Output

The trained LightGBM model is used to predict survival for the Titanic test dataset.

The predictions are saved as:

`submission.csv`

The file contains:

```text
PassengerId
Survived
```

## 📁 Files

```text
Titanic-Survival-Prediction-XGBoost-LightGBM/
│
├── XGBM_&_LGBM.ipynb
├── Titanic_train.csv
├── Titanic_test.csv
└── README.md
```

## ✅ Conclusion

This project demonstrates the complete machine learning workflow for Titanic survival prediction, including EDA, preprocessing, model development, evaluation, and hyperparameter tuning.

Both **LightGBM and XGBoost** are compared using multiple classification metrics. GridSearchCV is used to identify improved LightGBM hyperparameters. The project provides practical experience with advanced gradient boosting algorithms and their application to structured classification data.

