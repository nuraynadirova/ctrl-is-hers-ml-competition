# CTRL IS HERS - Machine Learning Competition

This repository contains my solution for the CTRL IS HERS Machine Learning Competition.

## Project Objective

The goal of the project is to predict whether an online news article will be popular or not.

The target variable is binary:

- `0` - Not popular
- `1` - Popular

The competition is evaluated using the ROC-AUC metric.

## Dataset

The dataset includes different features related to online news articles, such as:

- Article and title length
- Number of images and videos
- Publishing weekday
- News channel
- Keyword statistics
- Sentiment features
- Subjectivity features
- LDA topic features

## Data Preprocessing

The following preprocessing steps were applied:

- Converted `publish_date` to datetime format
- Extracted `month` and `day` from the publishing date
- Removed unnecessary ID and date columns
- Handled numerical missing values using median imputation
- Handled categorical missing values using the most frequent value
- Applied One-Hot Encoding to categorical features

## Models Tested

Several classification models were tested:

- Logistic Regression
- Extra Trees Classifier
- Random Forest Classifier
- Gradient Boosting Classifier

The models were compared using ROC-AUC.

## Validation Results

| Model | ROC-AUC |
|---|---:|
| Logistic Regression | 0.6281 |
| Extra Trees | 0.7097 |
| Random Forest | 0.7195 |
| Gradient Boosting | 0.7256 |

## Final Model

Gradient Boosting Classifier achieved the highest validation ROC-AUC score among the tested models, so it was selected as the final model.

## Kaggle Result

Public Leaderboard ROC-AUC:

**0.74835**

## Files

- `ctrl_is_hers_competition.ipynb` - data preprocessing, model training, evaluation and prediction
- `README.md` - project documentation

## Author

Nuray Nadirova
