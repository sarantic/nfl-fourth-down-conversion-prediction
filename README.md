# NFL Fourth-Down Conversion Prediction

A machine learning project that predicts the probability of a successful NFL fourth-down conversion using historical play-by-play data. The project develops a calibrated logistic regression model to estimate conversion probabilities based on game situation, field position, play type, and team information.

## Project Overview

NFL teams increasingly face difficult fourth-down decisions where the choice to "go for it" can significantly affect game outcomes. This project builds a predictive model that estimates the likelihood of converting a fourth down, providing a quantitative tool that could support play-calling and decision-making.

## Features

- Historical NFL fourth-down conversion dataset
- Data preprocessing and feature engineering
- One-hot encoding of categorical variables
- Logistic Regression classifier
- Probability calibration
- Model evaluation using classification and calibration metrics
- Visualization of model performance

## Technologies

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib
- Jupyter Notebook

## Repository Structure

```
.
nfl-fourth-down-conversion-prediction/
│
├── README.md                   
├── LICENSE                      
├── .gitignore
├── requirements.txt
├── notebooks/
│   └── fourth_down_analysis.ipynb
│
├── reports/
│   └── project.html             
│
├── models/
│   ├── model.joblib
│   └── calibrated_logreg.joblib
│
└── images/
    ├── probability_by_yards.png
    └── calibration_plot.png

```

## Model Inputs

The model predicts fourth-down conversion success using:

- Yards to first down (`togo`)
- Field position (`yardline`)
- Play type (run/pass)
- Offensive team
- Defensive team

## Objective

Estimate the probability that a fourth-down conversion attempt will succeed, enabling more informed strategic decision-making.

## Future Improvements

- Compare additional classification models (Random Forest, XGBoost, Neural Networks)
- Incorporate score differential and game clock
- Analyze feature importance
- Build an interactive dashboard for probability predictions
