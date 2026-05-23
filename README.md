# Road-Safety-Analysis

This repository contains an exploratory data analysis (EDA) and machine learning modeling of road safety and traffic crash data. The project aims to uncover insights into the factors contributing to traffic accidents, their severity, and other related parameters, and utilizes predictive modeling to analyze these factors.

## Overview
The analysis is conducted using a Jupyter Notebook (`V1.ipynb`). It processes the dataset, provides statistical summaries and visualizations, and applies multiple machine learning classifiers to understand the patterns in road accidents and identify the most critical risk factors.

## Dataset Features
The dataset analyzed includes the following features:
* **Crash_Severity**: The severity level of the crash (e.g., Minor injury)
* **Vehicle_Speed**: The speed of the vehicle involved
* **Crash_Time**: The time of day the crash occurred
* **Age & Gender**: Demographics of the individuals involved
* **Vehicle_Type**: The type of vehicle (e.g., Car)
* **Road conditions**: Number_of_Lanes, Lane_Width, Road_Type, Road_Surface_Condition
* **Other factors**: Alcohol_Consumption, Crash_Type, Seatbelt_Usage, Speed_Limit

## Algorithms & Machine Learning Models
The project implements several machine learning classifiers. The `lazypredict` library is initially used to rapidly evaluate the performance of numerous models simultaneously.

Based on the preliminary evaluation, the following specific algorithms were implemented and analyzed in detail (including the generation of Feature Importance visualizations):
* **Bagging Classifier**
* **Decision Tree Classifier**
* **Gradient Boosting Classifier**
* **Random Forest Classifier**
* **Extra Trees Classifier**

## Results & Outputs
* **Feature Importance:** The analysis successfully identifies the key features that contribute most significantly to road accidents. By leveraging the feature importance attributes of the tree-based models (like Random Forest and Gradient Boosting), the project highlights which variables (e.g., speed limit, crash time, road conditions) are the strongest predictors of crash outcomes.
* **Model Performance:** Various models were tested, with ensemble methods (such as LGBMClassifier and Random Forest) showing distinct predictive capabilities. The output includes performance metrics (like Accuracy and F1-score) for over 25 different classifiers.
* **Data Insights:** The exploratory data analysis uncovers underlying trends related to crash times, vehicle types, road conditions, and demographics, providing a comprehensive statistical view of the factors affecting road safety.

## Tools and Libraries
The project utilizes the following Python libraries:
* **Pandas & NumPy**: For data manipulation and statistical calculations
* **Seaborn & Matplotlib**: For data visualization
* **Scikit-learn & LazyPredict**: For predictive modeling and rapid model evaluation
* **SciPy**: For statistical tests

## Usage
To view the analysis, simply open the `V1.ipynb` notebook. The dataset is expected to be loaded as a CSV file.
