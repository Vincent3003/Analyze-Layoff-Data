# Predicting Layoff Patterns Based on Company Attributes

**Overview:** 
This project aims to explore and analyze layoff trends in companies across various industries, locations, and stages of growth using machine learning techniques. By leveraging models like decision trees, random forests, and linear regression, the project seeks to uncover patterns and factors associated with layoffs, providing insights into how different attributes impact workforce reductions

**Data:**
The project uses the Layoffs Dataset from Kaggle, containing information on 3,485 individuals. This dataset includes fields such as Company Name, Location (City and Country), Industry, and Total Number of Layoffs. Three versions of the dataset were prepared for analysis:
- layoff_data(3).csv: the original data from Kaggle.
- layoff_clean.csv: A cleaned version of the original data with standardized fields and corrected entries.
- layoff_USA_clean.csv: A filtered version of the cleaned data, including only entries for companies based in the USA.

**Methods:**
The analysis workflow includes the following:
- Data Cleaning: Performed in Python to ensure the accuracy and consistency of the dataset.
- Exploratory Data Analysis (EDA): Visualizations and exploratory analysis to identify trends and patterns in layoff data.
- Predictive Modeling: Utilizing linear regression, decision tree regression and random forest regression models to make insightful predictions and understand key factors influencing layoffs."

**Key Results:**
- Meta has the highest funds raised and the largest layoff count, both in the USA and globally.
- Quarter 1 of 2023 saw the highest number of layoffs worldwide and within the USA.
- The Retail, Consumer, and Other industries have the highest layoff counts, both globally and in the USA.
- San Francisco has the highest number of layoffs in the USA, likely due to the high concentration of companies in the area.

**Model Evaluation Results:**
- Linear Regression: This model had a very low R² score (close to zero) on both the training and test data, with an MSE of 494,584. This indicates that linear regression struggled to capture the relationships in the data, likely due to the complex or non-linear nature of layoff trends.
- Decision Tree: The decision tree model performed well, achieving high R² scores (0.995) on both the training and test data. This suggests that the decision tree effectively captured patterns in the layoff data. However, it’s still essential to be cautious of overfitting, as decision trees can sometimes memorize the training data.
- Random Forest: The random forest model showed a high R² score (0.850) on the training data but a significantly lower R² score (0.238) on the test data, with an MSE of 377,025. This discrepancy indicates that the random forest model may be overfitting and could benefit from further tuning to improve generalization to new data.

  **Recommendations:**
  - Focus on Optimizing Decision Tree Models: Given their superior performance, focus on refining decision trees as the primary model.
  - Implement Cross-Validation: Use cross-validation across all models to ensure robust performance and reduce overfitting.
  - Regularization Techniques for Linear Regression: Test Ridge or Lasso regression as alternatives to simple linear regression, as these techniques may improve generalization and handle multicollinearity.
