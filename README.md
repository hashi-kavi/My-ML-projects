# My-ML-projects
# 1.Medical Cost Prediction

This project implements a machine learning model to predict medical insurance costs based on personal characteristics and health indicators.

## Dataset

The project uses the Medical Cost Personal Dataset from Kaggle, which includes the following features:

- **age**: Age of primary beneficiary
- **sex**: Insurance contractor gender (female/male)
- **bmi**: Body mass index
- **children**: Number of children covered by health insurance
- **smoker**: Smoking status (yes/no)
- **region**: Residential area in the US (northeast, southeast, southwest, northwest)
- **charges**: Individual medical costs billed by health insurance (target variable)

## Project Structure

The project is implemented in a Jupyter notebook and follows these main steps:

1. **Data Loading and Initial Analysis**
   - Loading the dataset using pandas
   - Basic data exploration and shape analysis
   - Feature and target separation

2. **Data Preprocessing and EDA**
   - Train-test split (75%-25%)
   - Exploratory Data Analysis (EDA)
     - Numerical feature analysis
     - Distribution visualization
     - Gender and smoker distribution analysis
     - Charge distribution analysis
   - Feature preprocessing
     - One-hot encoding for categorical variables (sex, smoker, region)
     - MinMax scaling for numerical features (age, bmi)

3. **Model Implementation & Evaluation**
   - Linear Regression
   - Random Forest Regressor
   - Cross-validation
   - Model evaluation using:
     - R-squared score
     - Mean Squared Error

## Key Findings

The project implements and compares two models:
1. Linear Regression
2. Random Forest Regressor (with n_estimators=10, max_depth=5)

Both models are evaluated using 5-fold cross-validation to ensure robust performance assessment.

## Requirements

The project requires the following Python libraries:
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

## Usage

1. Ensure all required libraries are installed
2. Load the Jupyter notebook
3. Execute cells in sequence to:
   - Load and preprocess data
   - Train models
   - Evaluate performance

## Dataset Reference

Dataset source: [Kaggle - Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance/data)
