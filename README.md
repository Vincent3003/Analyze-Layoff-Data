# Predicting Layoff Patterns Based on Company Attributes

**🧠 Overview:** 
Explored and modeled layoff trends across industries, locations, and company stages using machine learning. Applied decision trees, random forests, and linear regression to uncover key predictors of layoffs and provide insights into workforce reduction patterns.

**📊Data:**
The project uses the Layoffs Dataset from Kaggle, containing information on 3,485 individuals. This dataset includes fields such as Company Name, Location (City and Country), Industry, and Total Number of Layoffs. Three versions of the dataset were prepared for analysis:
- layoff_data(3).csv: the original data from Kaggle.
- layoff_clean.csv: A cleaned version of the original data with standardized fields and corrected entries.
- layoff_USA_clean.csv: A filtered version of the cleaned data, including only entries for companies based in the USA.

**⚠️ Key challenges:**

- Identified top factors driving layoffs across industries and growth stages.
- Analyzed the impact of attributes like company location, funding levels, and industry type.
- Resolved issues related to missing values, data inconsistencies, and quality.

**🎯 Objectives:**

- Clean and preprocess the layoff data to ensure accuracy and consistency.
- Conduct exploratory data analysis (EDA) to identify initial patterns and insights in layoff trends.
- Develop predictive models using machine learning techniques to determine key factors affecting layoffs and to predict layoff trends based on company attributes.

** 🛠️ Method & Tools:**

- **Python:** Data cleaning, EDA, and predictive modeling.
- **ML Models:** Decision Tree, Random Forest, Linear Regression.
- **EDA:** Identified trends by industry, quarter, and geography.

**📈 Impact & Insights:**

- **Meta** led in total layoffs and funding raised (globally and in the USA).
- **Q1 2023** saw the highest global and U.S. layoff volume.
- **Retail, Consumer, and Other Industries** had the highest global layoff counts.
- **U.S.** led in total layoffs; San Francisco showed the highest city-level concentration.

**📌 Conclusion & Strategic Recommendations:**

- **✅ Conclusion:** Best Model is Decision tree (strong R² on train/test, best overall performance). Linear regression underperformed due to a non-linear data structure (low R², high MSE).
- **🔁 Recommendations:** Tune Random Forest to reduce overfitting (train R² = 0.850 vs test R² = 0.238); apply cross-validation across all models for robustness.
