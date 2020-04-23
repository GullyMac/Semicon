# Semiconductor Thin Film Thickness Prediction

This project is an entry for the 1st Monthly Data Analysis Competition organized by DACON.

DACON main : https://newfront.dacon.io/

Competition Info. : https://dacon.io/competitions/official/235554/overview/

Report : https://github.com/GullyMac/Semicon/blob/master/semicon.ipynb

20.04.23 last edit

---

## 0. Environment

* Language : Python
* Editor : Google Colaboratory (Jupyter Notebook)

   ! Performance can change depending on the hardware allocated by Colab.
* CPU : Intel® Xeon®
* RAM : about 25GB
* Disk : about 68GB
* GPU : Tesla P100

   ! When using GPU, there are a little of differences in result.

---

## 1. Introduction

#### Background:

Recently, as the demand for high-spec semiconductors has increased.

In the process of stacking semiconductor thin films, there are uniformity and thickness decrease problems due to films' defects.

It is important to measure the thickness of the thin film quickly and accurately, and we can solve this through big data analysis.

#### Organizer: DACON

#### Metric: MAE

---

## 2. Data Set

#### Data Sets are provided by DACON

#### Response Variable

* The thickness of the thin film (layer_1~4)

#### Explanatory Variable
* Reflectance spectrum, wavelength of light (0~225)

---

## 3. Library

#### Environment Setting

* google.colab.drive : mount at google drive
* warnings : ignore warning message
* os : directory setting

#### Data Manipulation

* pandas : data manipulation
* numpy : matrix operation
* random : random number generation
* time : time measurement

#### Visualization

* matplotlib.pyplot : graph drawing

#### Modeling

* sklearn.model_selection.train_test_split : seperate train and validation data set
* sklearn.model_selection.KFold : k-fold cross validation
* sklearn.metrics : residual measurement
* bayes_opt : Bayesian optimization
* functools.partial : freeze a function’s arguments
* keras

