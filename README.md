## CHD-Race-and-Sex-Analysis
Research Analysis of CHD and Race/Sex 

This research data is originally from my statistics class project, which utilizes a clinical dataset of 100 observations to investigate the primary demographic predictors of Coronary Heart Disease (CHD). Using Binomial Logistic Regression in jamovi, this analysis examines how variables such as Age, Sex, and Race influence the probability of a CHD diagnosis.

The goal of this project is to demonstrate competency in epidemiological data analysis, multivariate statistical modelling, and the interpretation of odds ratios (OR) in a public health context. 


With this dataset, I wanted to answer 2 questions: 

- Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? 

- Secondary: Is race also a significant factor for CHD? If so, which group is most prominent?




## 1) Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? Gender Specific Analysis



<img width="654" height="297" alt="image" src="https://github.com/user-attachments/assets/ff2d2835-09b7-4225-99ba-f8fbe67c2685" />


🔬 Methodology
- Model Type: Binomial Logistic Regression (Unadjusted)
- Dependent Variable: CHD Status ($0$ = Absent, $1$ = Present)Factor: Sex (Reference Level: Female)
- Statistical Power: The model is statistically significant ($\chi^2 = 16.3, p < .001$), explaining approximately $11.8\%$ of the variance in CHD status (McFadden’s $R^2 = 0.118$).



📊 Key Findings: The Gender Risk Gap
- The analysis revealed a stark and statistically significant difference in heart disease risk based on sex ($p < .001$).
- Odds Ratio (OR): 5.43Interpretation: Males in this sample are $5.43$ times more likely to have been diagnosed with Coronary Heart Disease compared to females.
- Confidence Interval: We are $95\%$ confident that the true increased risk for males falls between $2.30$ and $12.80$ times that of females.



📝 Discussion & ContextWhile the raw risk for males is over 5 times higher, this "unadjusted" model does not account for the fact that males in this dataset are significantly older than the females. This result serves as the "Baseline Comparison" before moving into the multivariate analysis where Age is controlled for.



      



## 2) Secondary: Is race also a significant factor for CHD? If so, which group is most prominent? 



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
