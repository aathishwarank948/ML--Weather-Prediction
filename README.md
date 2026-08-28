# Implementation of Random Forest Algorithm for Weather Prediction
## NAME : AATHISHWARAN K
## REGISTER NUMBER : 212225040006

## AIM:
To write a program to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data using Random Forest Algorithm.

## Problem Statement and Dataset

 

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
1) Load the weather dataset using pandas.
2) Preprocess the data by handling missing values and sorting by time.
3) Select features and create lag variables for temperature and PM2.5.
4) Train Random Forest models to predict temperature and PM2.5 and save the models.
```

## Program:
```
Program to implement the Random Forest Algorithm to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data.
Developed by: AATHISHWARAN K
Register Number: 212225040006
```
```py
# Implementation of Random Forest Algorithm for Weather Prediction

import pandas as pd
import matplotlib.pyplot as plt

from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score

# Load dataset
data = pd.read_csv("weather-station-eee-block_2024_07_13 (1).csv")

# Display first 5 rows
print("First 5 rows of the dataset:")
print(data.head())
