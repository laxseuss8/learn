##Crop Recommendation System using Soil Metrics

##Project Overview

This project assists farmers in selecting the optimal crop based on soil metrics (Nitrogen, Phosphorous, Potassium, and pH levels). Using machine learning, a multi-class logistic regression model evaluates the predictive power of each soil feature to determine which has the greatest impact on crop selection. The model identifies Potassium (K) as the most critical feature for accurate predictions.

##Dataset

File: soil_measures.csv

##Features:

N: Nitrogen content ratio

P: Phosphorous content ratio

K: Potassium content ratio

pH: Soil pH valueTarget: crop (categorical, 22 unique crops)

##Key Steps & Methodology

1. Data Exploration & Preprocessing

Checked for missing values (none found).

Visualized feature distributions using boxplots.

Split data into training (70%) and testing (30%) sets with stratification.

2. Model Training & Evaluation

Algorithm: Logistic Regression (multi-class).

Evaluation Metric: Weighted F1-score (accounts for class imbalance).

Each soil feature (N, P, K, pH) was tested individually to assess its predictive power.

3. Results

Feature

F1-Score

N

0.135

P

0.161

K

0.258

pH

0.089

##Conclusion: Potassium (K) is the most important feature for predicting the optimal crop.

##Code Structure

Data Loading & Exploration: Load dataset, inspect data, and visualize distributions.

Feature Analysis: calculate_feature_performance() trains and evaluates models for each feature.

Result Extraction: best_predictive_feature() identifies the top-performing feature.

##Usage

Requirements

Python 3.8+

Libraries: pandas, scikit-learn, seaborn, matplotlib

Run the Code

Ensure soil_measures.csv is in your working directory.

Execute the Jupyter notebook to:

Load and preprocess data.

Train models and evaluate features.

Output F1-scores and identify the best feature.

#Insights for Farmers

Focus on Potassium Levels: The model highlights Potassium as the strongest predictor of crop suitability. Farmers should prioritize measuring and optimizing K levels in their soil.

Cost-Efficiency: By identifying the most impactful metric, this system reduces the need for expensive comprehensive soil tests.
