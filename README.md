# Weather Data Analysis and Rainfall Prediction using Python

## Project Description

This project focuses on analyzing daily weather data and predicting rainfall using Python, Data Analysis, and Machine Learning techniques. The dataset contains various weather-related parameters such as temperature, humidity, atmospheric pressure, cloud cover, wind speed, and rainfall measurements.

The main objective of this project is to explore weather patterns, visualize trends, understand relationships between different weather conditions, and build a machine learning model to predict rainfall.

The project demonstrates a complete beginner-level data science workflow including:

- Data Collection
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Analysis
- Machine Learning Model Building
- Model Evaluation

---

# Objectives

The major objectives of this project are:

- To analyze daily weather conditions
- To identify trends and seasonal variations in weather data
- To visualize relationships between weather parameters
- To understand the impact of temperature, humidity, and pressure on rainfall
- To build a machine learning model for rainfall prediction
- To evaluate model performance using Mean Squared Error (MSE)

---

# Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Scikit-learn | Machine Learning |

---

# Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error
```

---

# Dataset Description

The dataset contains 366 daily weather observations with 22 weather-related features.

## Important Features

| Feature | Description |
|---|---|
| MinTemp | Minimum Temperature |
| MaxTemp | Maximum Temperature |
| Rainfall | Daily Rainfall Amount |
| Humidity9am | Humidity at 9 AM |
| Humidity3pm | Humidity at 3 PM |
| Pressure9am | Atmospheric Pressure at 9 AM |
| Pressure3pm | Atmospheric Pressure at 3 PM |
| Cloud9am | Cloud Cover at 9 AM |
| Cloud3pm | Cloud Cover at 3 PM |
| Temp9am | Temperature at 9 AM |
| Temp3pm | Temperature at 3 PM |

---

# Data Exploration Analysis

## Dataset Information

The dataset contains:

- 366 rows
- 22 columns
- Numerical and categorical weather attributes

The analysis shows that:

- Most columns contain complete data
- Some columns contain missing values
- Weather parameters vary significantly across observations

---

# Missing Value Analysis

The dataset contains missing values in columns such as:

- Sunshine
- WindGustDir
- WindDir9am
- WindSpeed9am

## Analysis

Missing values can reduce model performance and lead to inaccurate predictions. Therefore, handling missing data is an important preprocessing step in data analysis.

Possible approaches:
- Removing missing rows
- Replacing missing numerical values with mean/median
- Replacing categorical values using mode

---

# Statistical Analysis

## Temperature Analysis

### Minimum Temperature
- Average MinTemp: 7.26°C
- Lowest MinTemp: -5.3°C
- Highest MinTemp: 20.9°C

### Maximum Temperature
- Average MaxTemp: 20.55°C
- Lowest MaxTemp: 7.6°C
- Highest MaxTemp: 35.8°C

## Analysis

The weather data shows large temperature variation, indicating seasonal climate changes throughout the year.

---

# Rainfall Analysis

### Rainfall Statistics
- Average Rainfall: 1.42 mm
- Maximum Rainfall: 39.8 mm

## Analysis

Most days recorded little or no rainfall, while a few days experienced heavy rainfall. This indicates an uneven rainfall distribution.

---

# Humidity Analysis

### Humidity Levels
- Average Humidity at 9 AM: 72%
- Average Humidity at 3 PM: 44%

## Analysis

Humidity levels are generally higher during the morning and decrease in the afternoon due to increasing temperatures and evaporation.

---

# Wind Analysis

### Wind Speed
- Average Wind Gust Speed: 39.84 km/h
- Maximum Wind Gust Speed: 98 km/h

## Analysis

The dataset includes both calm and high-wind conditions, indicating varying atmospheric conditions.

---

# Cloud Cover Analysis

### Cloud Distribution
- Cloud values range from 0 to 8

## Analysis

Higher cloud cover is often associated with increased rainfall probability and reduced sunshine duration.

---

# Data Visualization Analysis

## Pair Plot

The pair plot was used to visualize relationships between:
- Minimum Temperature
- Maximum Temperature
- Rainfall

## Observations
- MinTemp and MaxTemp show positive correlation
- Rainfall distribution is highly skewed
- Rainfall does not strongly correlate with temperature alone

---

# Correlation Heatmap Analysis

A correlation heatmap was created to identify relationships between numerical features.

## Important Findings
- Humidity has positive correlation with rainfall
- Pressure shows negative correlation with rainfall
- Temperature variables are strongly correlated with each other

---

# Time-Series Trend Analysis

Monthly weather trends were visualized using line plots.

## Observations
- Temperature changes gradually over time
- Rainfall patterns fluctuate across months
- Seasonal weather variations are visible

---

# Machine Learning Model

## Algorithm Used

Linear Regression

## Objective

Predict rainfall using:
- Minimum Temperature
- Maximum Temperature
- Humidity
- Pressure
- Cloud Cover

---

# Model Training Process

The dataset was divided into:
- 80% Training Data
- 20% Testing Data

The Linear Regression model was trained using Scikit-learn.

---

# Model Evaluation

## Mean Squared Error (MSE)

```text
Mean Squared Error for Rainfall Prediction: 37.07
```

---

# Analysis of Output

The obtained Mean Squared Error (MSE) value is relatively high.

## Reason

Rainfall prediction is a complex problem influenced by multiple atmospheric conditions. Using only a few features and a simple Linear Regression model limits prediction accuracy.

## Observations
- Temperature alone is not sufficient for accurate rainfall prediction
- Humidity and cloud cover have stronger influence on rainfall
- Weather data contains nonlinear relationships

---

# Future Improvements

The project can be improved by:

- Using larger datasets
- Applying advanced machine learning models
- Using feature engineering techniques
- Adding weather API integration
- Building an interactive dashboard

## Advanced Algorithms
- Random Forest
- Decision Tree
- XGBoost
- Gradient Boosting

---

# Learning Outcomes

This project helped in understanding:

- Data preprocessing techniques
- Exploratory Data Analysis (EDA)
- Statistical analysis
- Data visualization
- Machine Learning workflow
- Regression modeling
- Model evaluation methods

---

# How to Run the Project

## Step 1

Upload the dataset (`weather.csv`) to Google Colab.

## Step 2

Install required libraries if needed:

```python
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Step 3

Run the Python code cells sequentially.

---

# Conclusion

This project demonstrates how Python and Machine Learning can be used to analyze weather data and predict rainfall patterns. The analysis provides useful insights into weather behavior and highlights the importance of data preprocessing, visualization, and feature selection in machine learning projects.

Although the Linear Regression model achieved moderate performance, the project establishes a strong foundation for more advanced weather prediction systems.
