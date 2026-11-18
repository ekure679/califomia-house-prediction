
#California House Price Prediction

This repository contains a machine learning project that predicts median house values in California districts using the classic California Housing Dataset.

Project Overview
The goal of this project is to build and evaluate a regression model capable of predicting house values based on census-level features like median income, house age, average rooms, population, and location (latitude/longitude).

Dataset Summary
The dataset is fetched directly via Scikit-Learn's fetch_california_housing and includes 20,640 records with the following 8 features:

MedInc: Median income in block group
HouseAge: Median house age in block group
AveRooms: Average number of rooms per household
AveBedrms: Average number of bedrooms per household
Population: Block group population
AveOccup: Average number of household members
Latitude: Block group latitude
Longitude: Block group longitude
Target variable:

MedHouseVal: Median house value for California districts (expressed in hundreds of thousands of dollars, e.g., $100,000)
Project Workflow
Data Loading & Exploration (EDA):
Inspected dataset structures, shapes, missing values, and duplication.
Plotted relationships between key features (e.g., Median Income vs. Median House Value).
Data Splitting:
Partitioned the dataset into an 80% training and 20% testing split.
Model Development:
Trained a standard Linear Regression model using Scikit-Learn.
Evaluation & Performance Analysis:
Analyzed training and testing performance using the  R2  (R-squared) metric.
Training  R2 : ~0.613
Testing  R2 : ~0.576
Residual Diagnostics:
Calculated the residuals ( yactual−ypredicted ).
Generated a Residual Scatter Plot, a Residuals Distribution Histogram, and a Normal Q-Q Plot to validate model assumptions (homoscedasticity, normality of errors).
