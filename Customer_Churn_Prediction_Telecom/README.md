### Telecom Customer Churn Prediction

#### Project Overview
In the telecommunications industry, predicting customer churn—when customers switch from one service provider to another—is crucial for retaining existing customers and reducing costs associated with acquiring new ones. This project utilizes the Telco Customer Churn dataset to explore factors influencing churn and develop predictive models.

#### Dataset Information
- **Dataset Name:** Telco Customer Churn
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Rows and Columns:** 7043 rows, 21 columns

#### Project Steps

1. **Data Preprocessing**
   - Converted `TotalCharges` column to float type.
   - Handled empty strings in `TotalCharges` by filling with 0.
   - Checked for null values and removed duplicates.
   - Dropped irrelevant columns (`customerID`).
   - Checked for outliers in numerical columns (`tenure`, `MonthlyCharges`, `TotalCharges`).

2. **Exploratory Data Analysis (EDA)**
   - Utilized univariate, bivariate, and multivariate analyses.
   - Descriptive statistics and visualizations (pie chart, bar chart, box plot, histograms, pair plot).
   - Identified key insights such as average tenure, monthly charges, total charges, and churn rate.

3. **Feature Engineering**
   - Encoded categorical data using label encoding and one-hot encoding.
   - Addressed multicollinearity by removing highly correlated columns.

4. **Model Selection and Training**
   - Split data into training and testing sets.
   - Trained multiple models: Logistic Regression, Gradient Boosting, and Random Forest.
   - Evaluated models based on accuracy and other metrics (precision, recall, F1 score).

5. **Model Evaluation**
   - Compared model performance using metrics and classification reports.
   - Selected Gradient Boosting as the top performer with an accuracy of approximately 81%.

#### Conclusion
In conclusion, this project demonstrated the significance of predicting customer churn in the telecom industry. By leveraging predictive analytics and understanding factors like tenure, monthly expenditure, and contract type, telecom companies can proactively manage customer retention strategies. The insights gained underscore the importance of data-driven decision-making to enhance customer loyalty and business sustainability.

This README provides a concise overview of the project's objectives, methodologies, and key findings, serving as a reference for stakeholders interested in understanding the telecom customer churn prediction process.
