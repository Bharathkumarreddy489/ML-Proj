# Hallucination Detection Model using Logistic Regression

## Overview
This repository contains a machine learning model built to detect hallucinatory text using logistic regression. The model analyzes textual data consisting of contexts, questions, and answers to predict whether a given text exhibits signs of hallucination.

## Dataset
The dataset used for training and evaluation is the "Hallucination-Dataset-400-Samples.csv". It includes the following columns:
- **Context:** Background information or context for the statement.
- **Question:** Question related to the context.
- **Answer:** Answer or statement that may or may not exhibit signs of hallucination.
- **Hallucination:** Binary label (0 or 1) indicating whether the statement is a hallucination (1) or not (0).

## Methodology

### Data Preprocessing
- **Handling Missing Values:** Any missing values in the dataset were filled with empty strings.
- **Splitting the Dataset:** The dataset was split into training (60%) and testing (40%) sets using `train_test_split` from `sklearn.model_selection`.

### Model Training
- **Preprocessing Pipeline:** Text data (`Context`, `Question`, `Answer`) was processed using TF-IDF vectorization within a `ColumnTransformer`.
- **Classifier:** Logistic Regression was chosen as the classifier due to its effectiveness in binary classification tasks.

### Hyperparameter Tuning
- **Grid Search:** Hyperparameters for TF-IDF vectorization (`ngram_range`) and logistic regression (`C`, `penalty`) were tuned using `GridSearchCV`.

## Evaluation Metrics
- **Accuracy:** 81.99%
- **AUC-ROC Score:** 80.91%
- **F1 Score:** 85.57%

### Performance on Test Set
- **Actual Hallucination (y_test):**
  - Class 1: 101 samples
  - Class 0: 60 samples
- **Predicted Hallucination (y_pred):**
  - Class 1: 100 samples
  - Class 0: 61 samples

## Results and Predictions

The `results_df` DataFrame contains the complete set of predictions alongside actual values (`Hallucination`) and the corresponding `Context`, `Question`, and `Answer` texts used for prediction.

## Conclusion

The logistic regression model achieved promising results in detecting hallucinatory text based on the provided dataset. It demonstrates good accuracy, AUC-ROC score, and F1 score, indicating its effectiveness in distinguishing between hallucinatory and non-hallucinatory statements.

