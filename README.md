Education and Income: An Empirical Analysis

Overview

This project examines the relationship between educational attainment and income outcomes using micro-level census data. 
The analysis explores how education relates to the likelihood of earning above a specified income threshold and assesses 
whether this relationship persists after accounting for demographic and labor supply factors.

The project is designed as an economics-informed data analysis, emphasizing exploratory analysis, regression modeling, 
and careful interpretation rather than causal claims.

Research Questions

How does educational attainment relate to income levels?
Do individuals with more years of education have a higher probability of earning above the income threshold?
How do demographic characteristics and work intensity interact with education in explaining income differences?

Dataset

The analysis uses the Adult Census Income dataset, obtained from Kaggle and originally derived from U.S. Census data.

Key variables include:

Education level and years of education
Age
Gender
Hours worked per week
Income category (above or below threshold)

Income is recorded as a binary indicator, which motivates the use of probability-based models.

Note: The dataset is not included in this repository.
It can be downloaded from Kaggle and placed in the project directory before running the notebook.

Methodology
1. Data Cleaning & Preparation

Handled missing values and inconsistent categorical formatting
Converted education into a numeric “years of education” measure
Constructed a binary income indicator
Created demographic control variables (e.g., gender dummy)

2. Exploratory Data Analysis (EDA)

Examined income distribution
Analyzed education distributions
Visualized income differences across education levels
Compared work intensity between income groups

3. Regression Analysis

Two regression specifications were estimated:

Baseline Model:
Linear probability model with years of education as the sole explanatory variable.

Controlled Model:
Extended specification including age, hours worked per week, and gender as controls.

Coefficient comparisons are used to assess how the estimated relationship between education and income changes 
when additional factors are accounted for.

4. Robustness Check

A logistic regression model is estimated as a robustness check to verify whether the qualitative findings are consistent under a nonlinear probability model.

Key Findings

Years of education is positively and statistically significantly associated with the probability 
of earning above the income threshold.

The estimated effect of education decreases slightly after adding demographic and labor supply controls, 
indicating modest confounding.

Even after controlling for age, work intensity, and gender, education remains 
strongly associated with higher income outcomes.

Logistic regression results confirm the qualitative findings from the linear probability model.

Limitations

The analysis is observational and does not establish causal effects.
Unobserved factors such as ability, family background, or education quality may bias estimates.
Income is measured as a binary category rather than a continuous wage variable.
The linear probability model has known limitations, including potential heteroskedasticity and predictions outside the [0,1] range.

Tools & Libraries

Python
pandas, numpy
matplotlib, seaborn
statsmodels
Google Colab

How to Run

Download the Adult Census Income dataset from Kaggle.
Place the CSV file in the project directory.
Open the notebook and run all cells from top to bottom.

Project Purpose

This project was created to demonstrate applied data analysis skills relevant to data analyst and economics-focused roles, 
including:

Data cleaning and validation
Exploratory analysis
Regression modeling
Model comparison and interpretation
Clear communication of results and limitations

Author

Sidharth
