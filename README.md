# Statistical-Learning-Project
## College Enrollment Forecasting Using Random Forest Regression

## Project Overview
This project aims to predict college enrollment using the "College" dataset from the ISLR2 package, which includes information on 777 U.S. institutions. The objective is to analyze how institutional characteristics such as applications received, acceptance rates, out-of-state tuition, room and board expenses, and graduation rates influence enrollment decisions. The project uses Random Forest Regression and Linear Regression models to enhance prediction accuracy and interpretability.

## Dataset
- **Source:** ISLR2 package (U.S. News & World Report, 1995)
- **Attributes:** 18 variables including applications received, acceptance rates, enrollment figures, tuition costs, room and board expenses, faculty qualifications, student-to-faculty ratios, alumni donations, and graduation rates.
- **Objective:** Predict college enrollment and analyze factors influencing students' decisions.

## Installation and Setup
**Prerequisites:**
- R (Version >= 4.0)
- Required libraries: `ISLR2`, `dplyr`, `MASS`, `e1071`, `caret`, `randomForest`, `ggplot2`, `gridExtra`, `corrplot`

## Data Preprocessing
- Converted categorical variables to numeric.
- Addressed skewness in continuous variables using log transformation.
- Normalized variables for consistency.
- Created new features like Acceptance Rate for enhanced prediction.

## Exploratory Data Analysis (EDA)
- Histograms for distribution analysis.
- Box plots to detect outliers.
- Scatter plots with regression lines to explore relationships.
- Correlation matrix and Principal Component Analysis (PCA) for multicollinearity check.

## Feature Engineering and Selection
- Applied backward selection to eliminate redundant or irrelevant features.
- Final model includes: 
  - Applications (Apps)
  - Acceptances (Accept)
  - Out-of-State Tuition (Outstate)
  - Room and Board Costs (Room.Board)
  - Graduation Rate (Grad.Rate)
  - Full-time Undergraduates (F.Undergrad)
  - Part-time Undergraduates (P.Undergrad)
  - Alumni Donation Percentage (perc.alumni)

## Modeling
- **Linear Regression:** Performed k-fold cross-validation to optimize model parameters.
- **Random Forest Regression:** 
  - Configured 500 trees with 10-fold cross-validation.
  - Evaluated model using RMSE, MAE, and R-squared metrics.

## Results
- **Linear Regression:** 
  - R-squared = 0.95
  - RMSE = 234.8179
- **Random Forest Regression:**
  - R-squared = 0.967
  - RMSE = 185.9107
  - Outperformed Linear Regression, providing better prediction accuracy and reduced error.

## Conclusion
The Random Forest model effectively predicts college enrollment and explains approximately 96.7% of the variance. The model highlights key factors influencing enrollment decisions, providing valuable insights for educational institutions. Future improvements could include testing advanced machine learning methods and integrating additional variables for enhanced performance.

## Technologies and Software Used
- **R Programming**
- **RStudio**
- **Machine Learning Models:** Random Forest, Linear Regression
- **Statistical Techniques:** Backward Selection, Cross-Validation, Principal Component Analysis (PCA)
- **Visualization:** ggplot2, gridExtra, corrplot

## Acknowledgements
Developed as part of the Statistical Learning course (MATH-50028-001) at Kent State University.

