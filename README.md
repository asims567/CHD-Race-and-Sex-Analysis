## CHD-Race-and-Sex-Analysis

This research data is originally from my statistics class project, which utilizes a clinical dataset of 100 observations to investigate the primary demographic predictors of Coronary Heart Disease (CHD). Using Binomial Logistic Regression in jamovi, this analysis examines how variables such as Age, Sex, and Race influence the probability of a CHD diagnosis. The goal of this project is to demonstrate competency in epidemiological data analysis, multivariate statistical modelling, and the interpretation of odds ratios (OR) in a public health context. With this dataset, I wanted to answer 2 questions: 

- Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? 
- Secondary: Is race also a significant factor for CHD? If so, which group is most prominent?




## 🔬 Methodology
Software: jamovi (Version 2.3)
Statistical Model: Binomial Logistic Regression
Dependent Variable: 
- CHD Status (Binary: 0 = No Disease, 1 = Presence of Disease)
- Covariates: Age (Continuous)
- Factors: Race (4 levels: AF, MA, O, W)
- Sex (Male, Female)






## 1) Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? Gender Specific Analysis


### Male to Female
<img width="654" height="297" alt="image" src="https://github.com/user-attachments/assets/ff2d2835-09b7-4225-99ba-f8fbe67c2685" />

(Fig. 1)





🔬 Methodology

- Model Type: Binomial Logistic Regression (Unadjusted)
- Dependent Variable: CHD Status ($0$ = Absent, $1$ = Present)
- Factor: Sex (Reference Level: Female)
- Statistical Power: The model is statistically significant ($\chi^2 = 16.3, p < .001$), explaining approximately $11.8\%$ of the variance in CHD status (McFadden’s $R^2 = 0.118$).

📊 Key Findings: The Gender Risk Gap

- The analysis revealed a stark and statistically significant difference in heart disease risk based on sex ($p < .001$).
- Odds Ratio (OR): 5.43; Interpretation: Males in this sample are $5.43$ times more likely to have been diagnosed with Coronary Heart Disease compared to females.
- Confidence Interval: We are $95\%$ confident that the true increased risk for males falls between $2.30$ and $12.80$ times that of females.

📝 Discussion & Context

- While the raw risk for males is over 5 times higher, this "unadjusted" model does not account for the fact that males in this dataset are significantly older than the females. This result serves as the "Baseline Comparison" before moving into the multivariate analysis where Age is controlled for.





### Female to Male

<img width="595" height="304" alt="image" src="https://github.com/user-attachments/assets/2547cf02-be86-4760-b275-6f635eeb2e06" />

(Fig. 2)





🔬 Methodology

- Model Type: Binomial Logistic Regression (Bivariate)
- Dependent Variable: CHD Status ($0$ = Absent, $1$ = Present)
- Factor: Sex (Reference Level: Male)
- Model Fit: The model is statistically significant ($\chi^2 = 16.3, p < .001$), with a McFadden’s $R^2$ of $0.118$.

📊 Key Findings: Reduced Odds in Females

- The model provides a statistically significant negative estimate for the Female group ($p < .001$), indicating a lower likelihood of disease compared to the male baseline.
- Odds Ratio (OR): 0.184; Interpretation: The odds of a female having CHD are $0.184$ times (or approximately $81.6\%$ lower than) the odds of a male having CHD.
- Baseline Odds (Intercept): The intercept $OR$ of $2.00$ indicates that for the reference group (Males), the odds of having CHD are $2:1$ (meaning they are twice as likely to have the disease as not to have it in this specific sample).
- Confidence Interval: The $95\%$ CI for the $OR$ is $[0.078, 0.434]$, which does not cross $1.0$, confirming a robust statistical effect.


📝 Statistical Insight: It is important to note that an Odds Ratio of $0.184$ is the mathematical reciprocal of the $5.43$ $OR$ found when Males were compared to Females ($1 / 5.43 \approx 0.184$). This demonstrates internal consistency in the data: while males have $5.4\times$ the risk of females, females have roughly $1/5$th the risk of males.

      







## 2) Secondary: Is race also a significant factor for CHD? If so, which group is most prominent? 





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
