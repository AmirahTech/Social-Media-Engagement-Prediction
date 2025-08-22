# Social-Media-Engagement-Prediction
Project Overview

This project predicts whether a social media post will have high engagement (likes, shares, comments) using machine learning. The goal is to demonstrate an end-to-end ML workflow, from data preprocessing to model evaluation and visualization.

Dataset

Public social media dataset (CSV) containing posts from multiple platforms: Instagram, Twitter, Reddit, YouTube.

Columns include: text_content, likes_count, shares_count, comments_count, hashtags, mentions, sentiment_score, brand_name, platform, etc.

Target variable: high_engagement (binary, 1 if engagement score > median, else 0).

Tools & Libraries

Python (Google Colab)

Pandas: data manipulation

NumPy: numeric operations

Matplotlib & Seaborn: visualization

Scikit-learn: machine learning models & evaluation

Project Steps

Data Upload & Cleaning

Loaded CSV and handled missing/NaN values.

Feature Engineering

Created engagement_score = likes + shares + comments

Generated high_engagement binary target

Added text_length, hashtag_count, mention_count, post_hour

Categorical Encoding

Converted platform and brand_name into numeric columns using one-hot encoding

Train/Test Split

Split data into 80% training and 20% testing sets

Model Training

Logistic Regression (baseline)

Random Forest Classifier (main model)

Evaluation

Accuracy, precision, recall, f1-score

Confusion matrix

Visualization & Insights

High vs low engagement by platform and brand

Text length vs engagement

Random Forest feature importance

Results

Random Forest Accuracy: ~52%

Key Features:

text_length, sentiment_score, platform, brand_name, hashtags, mentions, post_hour

Observations:

Longer posts tend to get slightly higher engagement

Platform and brand affect engagement distribution

The model is better than random guessing but real social media engagement is complex

Conclusion

This project demonstrates end-to-end ML workflow: preprocessing → feature engineering → model training → evaluation → visualization.

Although accuracy is modest (~52%), the focus is on interpreting features and understanding engagement patterns.

Future improvements could include text vectorization (TF-IDF), hyperparameter tuning, or advanced models like XGBoost.

How to Run

Open the notebook in Google Colab.

Upload the dataset when prompted.

Run all cells from top to bottom.
