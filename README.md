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
- Factors: Race (4 levels: AF = African American, MA = Mexican American, O = Others, W = White)
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
- Odds Ratio (OR): 0.184: The odds of a female having CHD are $0.184$ times (81.6% less than) the odds of  males having CHD.
- (Intercept): The intercept $OR$ of $2.00$ indicates that for the reference group (Males), the odds of having CHD are $2:1$ (Men are twice as likely to have the disease).
- Confidence Interval: The $95\%$ CI for the $OR$ is $[0.078, 0.434]$. 


📝 Statistical Insight: It is important to note that an Odds Ratio of $0.184$ is the mathematical reciprocal of the $5.43$ $OR$ found when Males were compared to Females ($1 / 5.43 \approx 0.184$). This demonstrates internal consistency in the data: while males have $5.4\times$ the risk of females, females have roughly 1/5th the risk of males.

      







## 2) Secondary: Is race also a significant factor for CHD? If so, which group is most prominent? 


<img width="595" height="330" alt="image" src="https://github.com/user-attachments/assets/f5e2627b-3f27-49be-8bc8-4eb76c37ce93" />

(Fig. 1) 



<img width="475" height="334" alt="image" src="https://github.com/user-attachments/assets/a5a884f8-237f-40a3-ba3d-a08bd035b63e" />

(Fig. 2) 



<img width="380" height="179" alt="image" src="https://github.com/user-attachments/assets/cf118eda-6751-4a3b-88bb-ac77090b818e" />

(Fig. 3) 



🔬 Methodology

- Model Type: Binomial Logistic Regression (Bivariate)
- Predictor: Race (Categorical)Reference Level: White (W)
- Model Significance: The model is statistically significant ($\chi^2 = 12.38, p = 0.006$), indicating that race is a meaningful predictor in this sample.


📊 Key Findings: Risk by Demographic Group

- The analysis identified a clear hierarchy of risk, with the African American and Mexican American groups showing the most prominent likelihood of disease.

1. Predicted ProbabilitiesThe Estimated Marginal Means represent the "real-world" probability of a person in each group having CHD based on this sample:
- AF (African American): 64.3% probability
- MA (Mexican American): 56.5% probability
- O (Other): 41.7% probability
- W (White): 20.0% probability (Baseline)


2. Relative Risk (Odds Ratios)Using the White (W) group as the benchmark, the Odds Ratios (OR) quantify how much higher the risk is for other groups:
- AF vs. W: Individuals in the AF group are 7.2 times more likely to have CHD ($p = 0.002$).
- MA vs. W: Individuals in the MA group are 5.2 times more likely to have CHD ($p = 0.012$).
- O vs. W: While the risk was 2.8 times higher, this result did not reach statistical significance ($p = 0.106$), suggesting a larger sample size may be needed for this specific subgroup.


📝 Conclusion: The data demonstrates that Race is a significant factor for CHD in this population, with the African American (AF) group being the most prominently affected. These findings highlight significant health disparities that warrant further investigation into contributing factors such as age distribution, socioeconomic variables, or access to preventative care.



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
