#  Food Waste Prediction in Restaurants Using Machine Learning

### A Supervised Learning Approach for Predicting Food Waste

**Author:** S. SARUYAN

---

##  Project Overview

Food waste is a major challenge in restaurant operations. Restaurants may prepare more food than required, resulting in unnecessary food waste.

This project uses **Machine Learning** to predict the amount of food wasted in a restaurant based on factors such as the number of guests, quantity of food, event type, storage conditions, purchasing history, seasonality, preparation method, geographical location, and pricing.

The project is formulated as a **Supervised Learning → Regression** problem because the target variable, **Wastage Food Amount**, is a continuous numerical value.

---

##  Project Objectives

The main objectives of this project are:

* Predict the **Wastage Food Amount**.
* Identify useful patterns related to food waste.
* Compare different regression models.
* Evaluate model performance using appropriate regression metrics.
* Support better food preparation and planning decisions.

---

##  Dataset

**Dataset:** Food Wastage Data in Restaurant

**Source:** Kaggle

The dataset contains **1,782 rows and 11 columns**.

### Features

The project uses restaurant-related features including:

* Number of Guests
* Quantity of Food
* Type of Food
* Event Type
* Storage Conditions
* Purchase History
* Seasonality
* Preparation Method
* Geographical Location
* Pricing

###  Target Variable

**Wastage Food Amount**

The target is continuous, making this a **regression problem**.

---

##  Machine Learning Workflow

The project follows a typical Machine Learning workflow:

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Missing Value Check
     ↓
Duplicate Check
     ↓
Categorical Encoding
     ↓
Outlier Analysis
     ↓
Feature Scaling
     ↓
Train / Test Split
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Food Waste Prediction
```

The presentation describes this as the planned preprocessing and modelling workflow.

---

##  Machine Learning Models

Two regression models were used for comparison.

### 1. Linear Regression

Linear Regression was used as a baseline model.

It is:

* Simple and interpretable
* Suitable for predicting continuous values
* Useful as a reference model
* Effective when relationships are approximately linear

### 2. Random Forest Regressor

Random Forest Regressor is an ensemble learning model that combines multiple decision trees.

It can:

* Capture non-linear relationships
* Model more complex patterns
* Provide a more flexible alternative to Linear Regression

The two models were selected to provide a comparison between a simple baseline and a more flexible ensemble model.

---

##  Model Evaluation

The models were evaluated using:

### MAE — Mean Absolute Error

Measures the average absolute difference between actual and predicted values.

**Lower MAE is better.**

### RMSE — Root Mean Squared Error

Penalizes larger prediction errors more strongly.

**Lower RMSE is better.**

### R² Score

Measures how much of the variation in the target variable is explained by the model.

**Higher R² is better.**

### Results

| Model             |      MAE |     RMSE | R² Score |
| ----------------- | -------: | -------: | -------: |
| Linear Regression | 4.139069 | 5.393619 | 0.730013 |
| Random Forest     | 1.972173 | 3.172878 | 0.906569 |

Based on these reported evaluation results, **Random Forest Regressor achieved better performance** than Linear Regression, with lower MAE and RMSE and a higher R² score.

---

##  Project Impact

A food-waste prediction system could help restaurants with:

* 📊 Better demand estimation
* 🍲 Better food preparation
* 📉 Reducing excess food
* ♻️ Reducing overall food waste
* 🧠 Supporting data-driven planning

The overall goal is to turn restaurant data into useful predictions that can support more efficient and sustainable operations.

---

##  Limitations

Some limitations of the project include:

* Dataset size and coverage
* Available features
* Data quality
* Model assumptions
* Generalization to other restaurants

These factors should be considered before applying the model to real-world restaurant environments.

---

##  Future Improvements

Possible future improvements include:

* Collect more real-world restaurant data.
* Add more relevant features.
* Perform further hyperparameter tuning.
* Test additional regression algorithms.
* Deploy the model as a prediction application.

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Google Colab
* Jupyter Notebook
* GitHub

---

##  Project Structure

```text
Food-Waste-Prediction/
│
├── Food_Waste_Prediction.ipynb
├── README.md
├── dataset/
│   └── food_wastage.csv
│
└── images/
    ├── eda.png
    └── actual_vs_predicted.png
```

---

##  Project Links

### Google Colab

Add your Google Colab notebook link here:

```text
YOUR_COLAB_LINK
```

### Kaggle Dataset

Add the original Kaggle dataset link here:

```text
YOUR_KAGGLE_DATASET_LINK
```

---

##  Author

**S. SARUYAN**

Machine Learning Project
**Food Waste Prediction in Restaurants Using Machine Learning**

---

##  Conclusion

This project demonstrates how supervised machine learning can be applied to restaurant data to predict food waste.

By comparing **Linear Regression** and **Random Forest Regressor**, the project shows how different regression approaches can be evaluated using MAE, RMSE, and R².

The reported results indicate that **Random Forest Regressor performed better for this dataset**, making it the stronger model among the two evaluated approaches.

The project can be further improved by using larger real-world datasets, additional features, hyperparameter tuning, and eventually deploying the model as a practical prediction application.
