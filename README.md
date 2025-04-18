# House Price Prediction: Advanced Regression Analysis

This repository contains my solution for the regression analysis project focusing on house price prediction using the Ames Housing dataset from Kaggle's "House Prices: Advanced Regression Techniques" competition.

## Project Overview

The goal of this project is to predict house sale prices using regression techniques. The dataset contains 79 explanatory variables describing various aspects of residential homes in Ames, Iowa. This project demonstrates the application of data cleaning, feature engineering, and regression modeling to develop accurate price predictions.

## Repository Structure

```
ml_regression_binware/
├── data/
│   ├── train.csv                  # Training data
│   ├── test.csv                   # Test data
│   └── data_description.txt       # Feature descriptions
├── regression_binware.ipynb       # Main Jupyter notebook with analysis
├── README.md                      # This file
├── peer_review.md                 # Peer review of another project
└── requirements.txt               # Project dependencies
```

## [View the Notebook](./regression_binware.ipynb)

Click the link above to view the complete analysis notebook.

## [View the Peer Review](./peer_review.md)

Click the link above to view my peer review of another student's project.

## Key Findings

- The most important predictors of house prices are overall quality (0.79 correlation), living area (0.71 correlation), and garage capacity (0.64 correlation)
- Linear models performed surprisingly well, with Linear Regression, Ridge Regression, and Gradient Boosting all achieving nearly identical R² scores of 0.904
- Feature engineering, especially log transformations of skewed variables, substantially improved model performance
- Polynomial features without proper regularization led to severe overfitting (R² of -7.52)

## Model Performance

Our top performing models achieved:
- R² Score: 0.904 (Linear Regression, Ridge Regression, Gradient Boosting)
- RMSE: Approximately $20,000-$21,000 (11-12% of the average home price)

## Setup and Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setting up the environment

1. Clone this repository:
```bash
git clone https://github.com/yourusername/ml_regression_binware.git
cd ml_regression_binware
```

2. Create a virtual environment:
```bash
# On Windows
python -m venv .venv
.venv\Scripts\activate

# On macOS/Linux
python3 -m venv .venv
source .venv/bin/activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Open `regression_binware.ipynb` to view the analysis

## Technologies Used

- Python
- pandas for data manipulation
- scikit-learn for modeling
- matplotlib and seaborn for visualization
- numpy for numerical computing

## Future Work

- Implement advanced feature engineering techniques
- Explore additional models like XGBoost and neural networks
- Conduct more thorough hyperparameter tuning
- Integrate external economic and geospatial data

## Dataset

The dataset is from the [Kaggle House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) competition, providing a comprehensive view of housing attributes and their relationship to sale price.

## Author

Binware - April 2025