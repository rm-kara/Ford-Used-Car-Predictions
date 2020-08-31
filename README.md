# Ford-Used-Car-Predictions

![GitHub repo size](https://img.shields.io/github/repo-size/rm-kara/Ford-Used-Car-Predictions)
![GitHub stars](https://img.shields.io/github/stars/rm-kara/Ford-Used-Car-Predictions)
![GitHub contributors](https://img.shields.io/github/contributors/rm-kara/Ford-Used-Car-Predictions)
![GitHub forks](https://img.shields.io/github/forks/rm-kara/Ford-Used-Car-Predictions)

## Table of contents
* [Project Overview](#project-overview)
* [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installing Requirements](#installing-requirements)
* [EDA Highlights](#eda-highlights)
* [Tested Models](#tested-models)
* [Model Performance](#model-performance)
* [Resources](#resources)

## Project Overview
In this project I worked with a data set that contains roughly **370000 used cars from Ebay-Kleinanzeigen**. I decided to focus on the **Ford** brand, the reduced data set contains roughly **25500 Ford used cars**.  
The data was cleaned using **Pandas** and **Numpy**, visualizations were developed with **Seaborn** and **Matplotlib**.  
Transformational steps such as encoding categorical- and numerical variables were implemented by using Scikit-learn's **Pipeline, OneHotEncoder, SimpleImputer and ColumnsTransformer** module.  
Finally, an **XGBRegressor** model was applied to predict used car prices of Ford cars.

## Getting Started

### Prerequisites
**Python Version:** 3.7  
**Packages:**
* pandas 1.1.0 
* numpy 1.19.1
* scikit-learn 0.23.2
* matplotlib 3.3.1
* seaborn 0.10.1
* xgboost

### Installing Requirements
To create a new anaconda environment, download [conda_requirements.txt](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/requirements/conda_requirements.txt) and enter the following command:  
```
<conda create --name <env> --file conda_requirements.txt>
```
To install the packages with pip, download [requirements.txt](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/requirements/requirements.txt) and enter the following command:  
```
<pip install -r requirements.txt>
```
## EDA Highlights
**Year of Registration and Price:** 
![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Distribution-year-price.png "Yeara and Price")
***
**Vehicle Mileage:**
![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Distribution-km.png "km Distribution")
***
**Vehicle Prices Of Mileage Groups:**
![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Price-over-km.png "Price over km")
***
**Vehicle types Price Ranges:**
![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Vehicle-types.png "Types and price range")
***
**Vehicle Models:**
![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Vehicle-Model-price.png "Model price range")

## Tested Models
* XGBRegressor

## Model Performance
**Results XGBRegressor:**
* Mean Absolute Error: 680.63€
* Mean Squared Error: 1296394.66€
* Root Mean Squared Error: 1138.59€
* R2 Score: 94%  

![alt text](https://github.com/rm-kara/Ford-Used-Car-Predictions/blob/master/img/charts/Model-predictions.png "Model Predictions")

## Resources
* Link to Data: 
    - [Kaggle Dataset](https://www.kaggle.com/orgesleka/used-cars-database)
