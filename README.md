# Housing Price Prediction Model

A machine learning project that predicts housing prices using regression techniques and feature engineering on real-world datasets.

## Overview

This project demonstrates a complete machine learning pipeline for housing price prediction, from data exploration to advanced model optimization. The model processes housing data with features like area, rooms, amenities, and location to predict property prices in USD.

## Dataset

The dataset contains 3,479 housing records with the following features:

- **Area**: Property area in square meters
- **Room**: Number of rooms
- **Parking**: Parking availability (boolean)
- **Warehouse**: Warehouse availability (boolean)
- **Elevator**: Elevator availability (boolean)
- **Address**: Property location
- **Price**: Property price in local currency
- **Price(USD)**: Property price in US dollars (target variable)

## Features

### Data Processing

- Missing value handling with median imputation
- Categorical encoding for location data
- Feature scaling using StandardScaler
- Outlier detection and removal

### Feature Engineering

- Area per room calculation
- Total amenities scoring
- Polynomial features (Area squared)
- Feature interactions (Area × Room)
- Luxury scoring based on area and amenities
- Location premium indicators
- Categorical binning for rooms and area

### Model Implementation

- Linear Regression (baseline)
- Ridge Regression (L2 regularization)
- Lasso Regression (L1 regularization)
- Random Forest Regressor
- Gradient Boosting Regressor

## Performance

The model achieved significant performance improvements through advanced techniques:

- **Baseline Linear Regression**: R² = 0.4398
- **Best Model (Gradient Boosting)**: R² = 0.7434
- **Performance Improvement**: 70% increase in explained variance

### Metrics

- **R² Score**: 0.7434
- **RMSE**: $44,930
- **MAE**: $26,171

## Key Features Identified

Feature importance analysis revealed the most influential factors:

1. Luxury score (41.1%)
2. Address encoding (36.7%)
3. Area per room ratio
4. Total amenities count
5. Property area


## Usage

The notebook is organized into sequential sections:

1. **Data Loading and Exploration**: Initial data analysis and visualization
2. **Data Preprocessing**: Cleaning and feature preparation
3. **Baseline Model**: Simple linear regression implementation
4. **Advanced Techniques**: Feature engineering and model optimization
5. **Model Comparison**: Performance evaluation across multiple algorithms
6. **Visualization**: Comprehensive results analysis

## Model Pipeline

1. **Data Preprocessing**

   - Convert data types
   - Handle missing values
   - Encode categorical variables

2. **Feature Engineering**

   - Create derived features
   - Apply polynomial transformations
   - Generate interaction terms

3. **Model Training**

   - Split data (80% train, 20% test)
   - Scale features
   - Train multiple algorithms

4. **Evaluation**
   - Calculate performance metrics
   - Analyze feature importance
   - Generate visualizations

## Results Visualization

The project includes comprehensive visualizations:

- Actual vs Predicted scatter plots
- Residuals analysis
- Feature importance charts
- Model performance comparisons
- Error distribution analysis

