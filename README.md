# Patient Survival Prediction | ICU Mortality Modeling

**Predicting Patient Mortality Using Clinical and Demographic Data with R**


## Project Overview

This healthcare-focused ML project aims to **predict the survival outcome** of patients admitted to the Intensive Care Unit (ICU), using a rich dataset with over **190 clinical features** from ~92,000 patients. The goal is to support **critical decision-making in hospitals** by modeling mortality risk using **statistical inference and machine learning techniques**.


## Objective

To classify whether a patient will survive (`hospital_death = 0`) or not (`hospital_death = 1`) based on variables like:
- Vitals (heart rate, glucose, BMI, creatinine)
- Diagnoses (hepatic failure, diabetes)
- ICU types and treatment metadata
- Demographics (age, gender, ethnicity)


## Key Techniques & Methodology

### Data Preprocessing
- Handled missing values and extreme outliers using EDA
- Analyzed skewed variables using median/mean comparisons
- Removed high multicollinearity using VIF and correlation matrices

### Feature Selection
- **Chi-Squared Test** for categorical feature impact
- **LASSO Regression** for variable selection
- **Stepwise Regression (AIC)** for optimal model simplification

### Model Building
- **Logistic Regression** (with L1/L2 regularization)
- **Decision Tree Classifier** (for interpretability in clinical settings)
- Evaluation via **ROC curve**, **accuracy**, and **AUC score**

### Key Hypothesis Testing
- Impact of **hepatic failure**, **diabetes**, and **ICU types** on mortality
- Age group and gender-based survival differences
- Ethnicity-specific outcome disparities


## Outcomes & Insights

- **Senior citizens showed the highest mortality rate** across the dataset.
- **Hepatic failure** and **diabetes mellitus** showed statistically significant association with hospital deaths.
- Some ICU types had **higher death probabilities**, influencing decisions about triage and treatment prioritization.
- **LASSO and stepwise regression** were effective in highlighting key predictors like age, BMI, glucose levels, and ICU type.


## Tech Stack

- **Language**: R  
- **Tools**: RStudio, Tidyverse, MASS, glmnet  
- **Techniques**: Logistic Regression, Stepwise AIC, LASSO, Chi-Square Test  
- **Domain**: Predictive modeling in healthcare


## Repository Structure

```
📦 Patient-Survival-Prediction/
├── PART - 1.Rmd                   # Data Cleaning, EDA, Feature Analysis
├── PART - 2.Rmd                   # Modeling, Evaluation, Hypothesis Testing
├── dataset.csv                    # ICU patient data (~92,000 records)
├── Part - 1.pptx                  # Visual Storytelling (EDA & Insights)
├── Part - 2.pptx                  # Modeling Results & Medical Implications
└── README.md                      # This file
```


## Use Case

This model can help:
- Triage ICU patients based on real-time survival risk
- Optimize ICU staffing and treatment priorities
- Generate medical research insights using data-backed survival patterns


## Author

**Surya Vamsi Patiballa**  
M.S in Data Science – George Washington University

- Email  :-  svamsi2002@gmail.com
- LinkedIn  :-  https://www.linkedin.com/in/surya-patiballa-b724851aa/
- Resume  :-  https://drive.google.com/file/d/178IYcArC6YYVdJiIwRmJYodzKZ-JXe-D/view?usp=sharing
