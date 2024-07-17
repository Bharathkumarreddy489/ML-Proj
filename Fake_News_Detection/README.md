# Fake News Detection using Machine Learning

## Overview
This project aims to detect fake news articles using machine learning techniques. The dataset consists of text data from both fake and true news articles, and we employ various machine learning algorithms to classify and distinguish between them.

## Dataset
The dataset used for this project contains:
- **Fake News**: Articles that are intentionally misleading or false.
- **True News**: Articles that are factually accurate and truthful.

## Project Structure
- **Data Cleaning and Preparation**: The dataset is cleaned, and text preprocessing techniques are applied, such as converting to lowercase, removing punctuation and stopwords.
- **Exploratory Data Analysis (EDA)**: Basic exploration is performed to understand the distribution of articles across different subjects and the frequency of words in both fake and true news articles.
- **Feature Extraction**: CountVectorizer and TfidfTransformer are used to convert text data into numerical features suitable for machine learning models.
- **Model Building and Evaluation**: Several machine learning algorithms including Naive Bayes, Logistic Regression, Decision Tree, and Random Forest are trained and evaluated for their accuracy in classifying news articles.
- **Results**: Performance metrics like accuracy, precision, recall, and F1 score are analyzed, and confusion matrices are visualized to understand model predictions.

## Machine Learning Models Used
- **Naive Bayes**: A probabilistic classifier based on applying Bayes' theorem with strong (naive) independence assumptions.
- **Logistic Regression**: A linear model used for binary classification tasks, which predicts the probability of occurrence of an event.
- **Decision Tree**: A non-linear model that uses a tree-like graph of decisions and their possible consequences, which is suitable for capturing complex relationships.
- **Random Forest**: An ensemble learning method that constructs multiple decision trees and merges them together to get a more accurate and stable prediction.

## Conclusion
- The Decision Tree model achieved the highest accuracy of 99.67% in classifying fake and real news articles.
- Logistic Regression, Decision Tree, and Random Forest also performed well, demonstrating high accuracy and robustness.
- Each model has its strengths: Decision Tree for its interpretability, Logistic Regression for its simplicity, and Random Forest for its ensemble learning capability.

