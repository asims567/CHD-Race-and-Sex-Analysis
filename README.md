# CHD-Race-and-Sex-Analysis
Research Analysis of CHD and Race/Sex 

This research project utilizes a clinical dataset of 100 observations to investigate the primary demographic predictors of Coronary Heart Disease (CHD). By employing Binomial Logistic Regression within the jamovi statistical environment, this analysis identifies how variables such as Age, Sex, and Race influence the probability of a CHD diagnosis.

The goal of this project is to demonstrate competency in epidemiological data analysis, multivariate statistical modelling, and the interpretation of odds ratios (OR) in a public health context.



## 🔬 Methodology
Software: jamovi (Version 2.3)
Statistical Model: Binomial Logistic Regression
Dependent Variable: 
- CHD Status (Binary: 0 = No Disease, 1 = Presence of Disease)
- Covariates: Age (Continuous)
- Factors: Race (4 levels: AF, MA, O, W)
- Sex (Male, Female)




## Data Set

| CHD | Race | Sex | Age |
|----:|:-----|:----|----:|
|   1 | W    | F   |  25 |
|   1 | W    | F   |  30 |
|   1 | W    | F   |  34 |
|   1 | W    | F   |  36 |
|   1 | W    | F   |  37 |
|   1 | AF   | F   |  39 |
|   1 | AF   | F   |  40 |
|   1 | AF   | F   |  42 |
|   1 | AF   | F   |  43 |
|   1 | AF   | F   |  44 |
|   1 | AF   | F   |  44 |
|   1 | AF   | F   |  45 |
|   1 | AF   | F   |  46 |
|   1 | AF   | F   |  47 |
|   1 | AF   | M   |  48 |
|   1 | AF   | M   |  48 |
|   1 | AF   | M   |  49 |
|   1 | AF   | M   |  50 |
|   1 | AF   | M   |  52 |
|   1 | AF   | M   |  53 |
|   1 | AF   | M   |  53 |
|   1 | AF   | M   |  54 |
|   1 | AF   | M   |  55 |
|   1 | O    | M   |  55 |
|   1 | O    | M   |  56 |
|   1 | MA   | M   |  56 |
|   1 | MA   | M   |  56 |
|   1 | MA   | M   |  55 |
|   1 | MA   | M   |  55 |
|   1 | MA   | M   |  56 |
|   1 | MA   | M   |  56 |
|   1 | MA   | M   |  56 |
|   1 | MA   | M   |  57 |
|   1 | MA   | M   |  57 |
|   1 | MA   | M   |  57 |
|   1 | MA   | M   |  57 |
|   1 | MA   | M   |  58 |
|   1 | MA   | M   |  58 |
|   1 | O    | M   |  59 |
|   1 | O    | M   |  59 |
|   1 | O    | M   |  60 |
|   1 | O    | M   |  61 |
|   1 | O    | M   |  62 |
|   1 | O    | M   |  62 |
|   1 | O    | M   |  63 |
|   1 | O    | M   |  69 |
|   0 | O    | M   |  58 |
|   0 | O    | M   |  60 |
|   0 | O    | M   |  57 |
|   0 | O    | M   |  57 |
|   0 | W    | F   |  20 |
|   0 | W    | F   |  23 |
|   0 | W    | F   |  24 |
|   0 | W    | F   |  25 |
|   0 | W    | F   |  26 |
|   0 | W    | F   |  26 |
|   0 | W    | F   |  28 |
|   0 | W    | F   |  28 |
|   0 | W    | F   |  29 |
|   0 | W    | F   |  30 |
|   0 | W    | F   |  30 |
|   0 | W    | F   |  30 |
|   0 | W    | F   |  30 |
|   0 | W    | F   |  30 |
|   0 | W    | F   |  32 |
|   0 | W    | F   |  32 |
|   0 | W    | F   |  33 |
|   0 | W    | F   |  33 |
|   0 | W    | F   |  34 |
|   0 | W    | F   |  34 |
|   0 | AF   | F   |  34 |
|   0 | AF   | F   |  34 |
|   0 | AF   | F   |  35 |
|   0 | AF   | F   |  35 |
|   0 | AF   | F   |  36 |
|   0 | AF   | F   |  36 |
|   0 | AF   | F   |  37 |
|   0 | AF   | F   |  37 |
|   0 | AF   | F   |  38 |
|   0 | AF   | F   |  38 |
|   0 | MA   | F   |  39 |
|   0 | MA   | F   |  40 |
|   0 | MA   | F   |  41 |
|   0 | MA   | F   |  41 |
|   0 | MA   | F   |  42 |
|   0 | MA   | F   |  42 |
|   0 | MA   | F   |  42 |
|   0 | MA   | F   |  43 |
|   0 | MA   | M   |  43 |
|   0 | MA   | M   |  44 |
|   0 | O    | M   |  44 |
|   0 | O    | M   |  46 |
|   0 | O    | M   |  47 |
|   0 | O    | M   |  47 |
|   0 | O    | M   |  48 |
|   0 | O    | M   |  49 |
|   0 | O    | M   |  49 |
|   0 | O    | M   |  50 |
|   0 | O    | M   |  52 |
|   0 | O    | M   |  55 |








## 📊 Key Findings

The final model was highly significant **($\chi^2 = 89.6, p < .001$)** with a McFadden $R^2$ of 0.650, indicating strong predictive power. 
- Age as a Primary Driver: Age proved to be the most significant predictor **($p < .001$)**. For every one-year increase in age, the odds of having CHD increase by **77.9% (OR = 1.779)**.
  
- Demographic Variance: When adjusting for age, significant differences were observed across racial groups, highlighting the importance of demographic adjustment in clinical risk assessment.

- Model Accuracy: The classification table indicated an overall predictive accuracy of 86.9%, successfully identifying high-risk individuals based on the provided parameters.
