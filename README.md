# Bank Marketing Campaign Analysis

## Project Overview

This project focuses on analyzing and optimizing a bank's marketing campaign for fixed-term deposits using machine learning techniques. The primary objective is to develop a predictive system that accurately forecasts whether a customer will subscribe to a term deposit based on historical data and customer behavior. This approach aims to enhance campaign efficiency, minimize marketing waste, and increase conversion rates.

## Business Understanding

### Business Statement
In the competitive banking industry, fixed-term deposits are a well-known financial product requiring customers to lock in money for a specified period in exchange for a fixed interest rate.

### Business Problem
XY Bank's campaigns to encourage fixed-term deposits have led to significant waste due to many uninterested customers. The bank's marketing team has enlisted the Data Science Team to develop a predictive system to forecast customer deposits based on historical data and behavior, aiming to minimize errors and make campaigns more efficient and cost-effective.

## Analytical Approach

### Selection and Relevance of Evaluation Metrics
Precision is chosen as the primary metric because it measures the accuracy of positive predictions, directly correlating with reducing wasteful marketing expenditures. A high precision rate ensures that the marketing budget targets individuals most likely to respond positively, thereby maximizing ROI.

### Reason for Using Machine Learning Classification
Machine learning classification is essential because it can analyze large volumes of customer data to identify patterns and predict customer behavior more accurately than traditional methods. This helps minimize marketing waste and increase conversion rates.

### Goals
- **Optimize Marketing Budget:** Targeting the right customers reduces overall campaign costs.
- **Drive Revenue Growth:** Precision in targeting boosts revenue by focusing efforts on the most likely to convert customers.

## Data Understanding

### Feature Information
The dataset includes various customer attributes such as age, job, balance, housing, loan, contact method, month, campaign, pdays, and poutcome.

### Data Cleaning
Steps include handling missing values, encoding categorical variables, and scaling numerical features.

### Outliers
Identified and analyzed outliers in features like age, balance, campaign, and pdays to understand their impact on the model.

### Correlation
No single column has a high correlation with deposits, indicating multiple factors influence customer behavior. A moderate positive correlation exists between pdays and deposit (0.22).

## Modeling

### Initial Model Training
We initially trained several models, including Gradient Boosting Classifier, which showed the highest precision.

### Feature Selection
Recursive Feature Elimination (RFE) was used to select the most significant features, enhancing model performance.

### Hyperparameter Tuning
Performed using GridSearchCV to find the best combination of parameters, maximizing the precision score.

### Threshold Optimization
Adjusted the decision threshold to maximize precision, minimizing false positives, and ensuring targeted marketing.

## Evaluation

### Model Evaluation
- **Before Model:** Net Revenue: Twenty-eight thousand seven hundred forty-eight dollars and eight cents, ROI: Six hundred eighty-seven point two percent.
- **After Model:** Net Revenue: Eight thousand eight hundred fifteen dollars and eight cents, ROI: Fifteen hundred seventeen point six percent.
- **Precision:** Increased from seventy-eight point seventy-four percent to ninety-one point twenty-three percent.

## Conclusion

### Solutions Provided
Developed a predictive system using a Gradient Boosting Classifier, improving precision and optimizing the marketing strategy.

### Measurable Solutions
Highlighted significant cost savings and higher profit efficiency through ROI calculations and precision improvements.

### Recommendations for Business
- Minimize marketing waste.
- Increase conversion rates by focusing on high-probability customers.
- Optimize the marketing budget and drive revenue growth.

### Recommendations for Model Improvement
- Regularly update the model with new data to maintain accuracy.
- Explore additional features and data sources to enhance the model's predictive power.
- Conduct further validation and testing to ensure robustness across different customer segments and market conditions.

## Repository Structure
- `data/`: Contains the dataset used for the analysis.
- `notebooks/`: Jupyter notebooks documenting the data analysis, modeling, and evaluation process.
- `models/`: Saved model files for the final trained models.
- `scripts/`: Python scripts for data processing, model training, and evaluation.

## How to Run
1. Clone the repository.
2. Install the necessary dependencies.
3. Run the Jupyter notebooks or scripts in the specified order to reproduce the analysis and results.

## Authors
- Ammar Muzaki


