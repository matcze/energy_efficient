# Energy Efficiency Prediction – Machine Learning Project

## Overview

This project focuses on predicting **building energy efficiency** using machine learning models. The goal is to analyze how building design parameters affect **heating and cooling energy requirements**.

The project demonstrates two common machine learning problem types:

* **Regression** – predicting continuous energy load values
* **Binary Classification** – predicting whether the energy load is **high or low**

The analysis includes:

* Exploratory Data Analysis (EDA)
* Data preprocessing
* Model training and evaluation
* Comparison of multiple machine learning algorithms

Two notebooks were created to address both problems separately.

---

## Dataset

The dataset comes from the **UC Irvine Machine Learning Repository**.

Dataset characteristics:

* **768 samples**
* **10 columns**
* **8 input features**
* **2 target variables**

  * Heating Load
  * Cooling Load

The dataset represents different **building design configurations** and their corresponding energy efficiency values.

Because the dataset is relatively small compared to many machine learning datasets, careful preprocessing and model selection were required.

---

## Machine Learning Tasks

### 1. Regression

Regression models are used to predict **continuous numerical values**.

In this project, regression models predict:

* Heating Load

Notebook:

```
energy_efficient.ipynb
```

---

### 2. Binary Classification

To demonstrate classification techniques, the regression labels were converted into **binary classes** using the **median value as a threshold**.

* Values **above the median → High energy load**
* Values **below the median → Low energy load**

Notebook:

```
energy_efficient_class.ipynb
```

---

## Data Preprocessing

Key preprocessing steps included:

* **Feature Scaling**

  * Numerical features were standardized.

* **Categorical Encoding**

  * Two ordinal categorical variables were encoded using **One-Hot Encoding**.

* **Train/Test Split**

  * The dataset was divided into:
  * Training set
  * Test set

Because of the small dataset size, no separate validation set was used.

---

## Models Used

Several machine learning models were tested and compared.

### Regression Models

* Linear Regression
* SGDRegressor
* Ridge
* Lasso 
* ElasticNet
* Decision Tree Regressor
* Random Forest Regressor
* Gradient Boosting / XGBoost Regressor
* Neural Network implemented with **TensorFlowe**
* Neural Network implemented with **PyTorch**

### Classification Models

* Logistic Regression
* K-Nearest Neighbors
* Naive Bayes
* Decision Tree
* Random Forest Classifier
* Support Vector Machine (SVC)
* XGBoost Classifier
* Neural Network implemented with **PyTorch**

---

## Results

The dataset shows **strong correlations between building design features and energy loads**, which makes the prediction task relatively straightforward for many machine learning models.

Key observations:

* Most models achieved **very strong predictive performance**
* Classification models achieved **accuracy above 99%**
* Tree-based models and ensemble methods performed particularly well

---


Example libraries used:

* numpy
* pandas
* scikit-learn
* matplotlib
* seaborn
* xgboost
* **PyTorch**
* **TensorFlow**

---

## Skills Demonstrated

This project demonstrates practical machine learning workflow:

* Data Analysis (EDA)
* Data Preprocessing
* Regression Modeling
* Classification Modeling
* Model Evaluation
* Neural Networks with **PyTorch**

---

## Future Improvements

Possible future improvements include:

* Cross-validation for more robust evaluation
* Hyperparameter optimization
* Feature importance analysis
* Model explainability (SHAP / LIME)
* Deployment as a simple API

---