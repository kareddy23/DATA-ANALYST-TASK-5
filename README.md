# Task 5 - Exploratory Data Analysis (EDA)

## Overview
This project performs an in-depth Exploratory Data Analysis (EDA) on the famous Titanic dataset. It focuses on extracting key insights, identifying trends, and visualizing relationships using Python libraries.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn

## 2. Dataset Overview
- **Rows:** 891
- **Columns:** 12

Key columns include:
- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class
- `Sex`: Gender
- `Age`: Age in years
- `Fare`: Passenger fare

## 3. Data Quality Check
- Missing values detected in `Age`, `Cabin`, and `Embarked`.
- `Cabin` has significant missing data.

## 4. Univariate Analysis
- **Age Distribution**: Right-skewed distribution with most passengers between 20-40 years.
- **Survival Count**: 62% did not survive, 38% survived.
- **Gender Distribution**: Slightly more males than females.

- ## 5. Bivariate Analysis
- **Survival by Gender**:
  - Females had a much higher survival rate than males.
- **Survival by Passenger Class**:
  - 1st class passengers had higher survival rates compared to 2nd and 3rd classes.
- **Age vs Survival**:
  - Younger passengers (especially children) had higher survival probabilities.

## 6. Multivariate Analysis
- **Pairplot**:
  - Strong relationship observed between Fare, Pclass, and Survival.
- **Heatmap**:
  - Negative correlation between Pclass and Fare.
  - Positive correlation between Fare and Survival.

## 7. Handling Skewed Data
- **Fare** was highly skewed.
- Applied log transformation using `np.log1p(Fare)` to normalize distribution.

## 8. Key Findings
- Females had a significantly higher chance of survival.
- Younger individuals and passengers in higher classes were more likely to survive.
- Fare prices and class were important factors in survival.
- Data skewness (especially in Fare) needs transformation for modeling.

- ## 9. Conclusion
This exploratory analysis provided valuable insights into factors affecting survival on the Titanic. Observations from EDA can guide further feature engineering and model building.

---
