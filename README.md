# MU_PDS-01_Prosenjit_16_BostonHousingModeling

## Project Overview
This project performs a regression analysis using the Boston Housing dataset to predict housing prices based on various features. Two regression models are applied: **Linear Regression** and **Gradient Boosting Regressor**. The project includes data preprocessing, model training, evaluation, and visualization of results. 

The analysis is designed to provide insight into factors that affect housing prices and includes hyperparameter tuning for model optimization.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Dataset
The [Boston Housing dataset](https://www.kaggle.com/kashyapankush/boston-housing-dataset) contains information about housing in Boston, including attributes such as crime rate, average number of rooms, and distance to employment centers. The target variable is the median home value (`MEDV`).

## Requirements
To run this project, you’ll need:
- Python 3.x
- Libraries: 
  - `kagglehub` (for downloading the dataset)
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

## Installation
**Install the required Python libraries:**
pip install -r requirements.txt

**Download the Dataset using kagglehub:**
path = kagglehub.dataset_download("kashyapankush/boston-housing-dataset")
If using Google Colab, ensure you have the Kaggle API key in your environment for seamless dataset access.

**Project Structure**

├── README.md                   # Project documentation
├── main.ipynb                  # Jupyter Notebook with full analysis
├── requirements.txt            # Dependencies
└── images/                     # Folder for images used in the README
Usage
Open and run main.ipynb in Jupyter Notebook or Google Colab. Follow the steps to complete the data preprocessing, model training, and evaluation.

**Key Steps in the Analysis**
Data Loading: Load the dataset using kagglehub.
Exploratory Data Analysis (EDA): Explore data, check for missing values, and visualize correlations with a heatmap.
Data Preprocessing: Scale features and split data into training and test sets.
Model Training: Train two models, Linear Regression and Gradient Boosting Regressor, and evaluate performance using R² and Mean Squared Error.
**Hyperparameter Tuning:** 
Apply GridSearchCV to optimize model parameters.
Cross-Validation: Assess model stability with cross-validation.
Visualization: Plot actual vs predicted values and feature importance.
**Results**
The analysis reveals insights into which features have the most significant impact on housing prices, with Gradient Boosting providing better accuracy than Linear Regression. Detailed model performance metrics and visualizations are provided in the notebook.
