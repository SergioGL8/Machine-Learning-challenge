# Machine Learning Homework - Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

## Analysis

### Preprocessing
* First I assigned the `koi_disposition` as "y" (target) value and the rest columns as "X" (features).
* Then, I scaled and encoded the X and y values, finally split them into training and testing data.

### Tuning the models
* Using `GridSearchCV` to tune the model's parameters.

## Model Comparison

### Models

#### Random Forest
* Training Data Score: `1.0`, Testing Data Score: `0.905`
* Best Score after Hyperparameter Tuning: `0.887`

#### Support Vector Machine
* Training Data Score: `0.845`, Testing Data Score: `0.841`
* Best Score after Hyperparameter Tuning: `0.882`

#### Logistic Regression
* Training Data Score: `0.850`, Testing Data Score: `0.843`
* Best Score after Hyperparameter Tuning: `0.878`

#### K Nearest Neighbor
* Training Data Score: `0.876`, Testing Data Score: `0.836`
* Best Score after Hyperparameter Tuning: `0.832` (where `k=3`)

### Model Selection
Comparing all models, the random forest yielded the highest score after hypterparameters tuning. Therefore, the random forest model is better than the other three models.


- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -

##### © 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
