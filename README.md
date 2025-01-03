# Drug-Review-Analysis-Randomization-and-Machine-Learning

## Overview
This project explores the relationship between drug review display order and user satisfaction ratings and applies machine learning to predict whether a review belongs to the control or treatment group. The analysis involves:

1. **Randomization Experiment**: Testing whether the order in which reviews are displayed affects user satisfaction ratings.
2. **Machine Learning Analysis**: Building models to predict review group membership (control or treatment) based on features like `EaseofUse`, `Effectiveness`, and `Satisfaction`.

## Objectives
1. **Randomization Study**: 
   - Evaluate the impact of review order on user satisfaction.
   - Compare satisfaction ratings between control (random order) and treatment (sorted by `EaseofUse` or `Effectiveness`) groups.

2. **Machine Learning**:
   - Train models to classify reviews into control or treatment groups.
   - Explore the predictive power of features such as `EaseofUse`, `Effectiveness`, and `Satisfaction`.

## Dataset
- The dataset is hosted externally due to size constraints.
- Download it (https://drive.google.com/file/d/1NmrYgCuVpEHqPeZyBfWEt389hsiYFYo9/view?usp=sharing)

The dataset includes the following columns:
- `Age`: Age of the reviewer.
- `Condition`: Condition being treated.
- `DrugId`: Identifier for the drug.
- `EaseofUse`: Ease of use rating (1-5 scale).
- `Effectiveness`: Effectiveness rating (1-5 scale).
- `Satisfaction`: Satisfaction rating (1-5 scale).
- `Groups`: Control or treatment group (randomized).

## Methodology

### 1. Randomization Study
- **Hypothesis**: The order of reviews affects user satisfaction.
- **Groups**:
  - **Control Group**: Reviews are displayed in a random order.
  - **Treatment Group**: Reviews are sorted by `EaseofUse` or `Effectiveness`.
- **Analysis**: Independent t-tests and visualization (boxplots) to compare satisfaction ratings between groups.

### 2. Machine Learning
- **Objective**: Predict group membership (`control` or `treatment`) based on features.
- **Models**:
  - Logistic Regression
  - Random Forest Classifier
- **Evaluation Metrics**:
  - Accuracy
  - Precision, Recall, and F1-Score
  - Feature Importance Analysis

## Results
1. **Randomization Study**:
   - Boxplots showed minimal differences in satisfaction ratings between the control and treatment groups.
   - Statistical tests revealed no significant effect of review order on satisfaction.

2. **Machine Learning**:
   - Logistic Regression and Random Forest models achieved comparable accuracy (~50%).
   - Feature importance analysis suggested weak predictive power of the features.

## License
This project is licensed under the MIT License. 

## Acknowledgments
- Data sourced from WebMD user reviews provided by Kaggle.
- Analysis inspired by randomized experimental design and machine learning classification methods.
