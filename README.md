[CHD_M-F_Analysis.html](https://github.com/user-attachments/files/26980248/CHD_M-F_Analysis.html)# CHD-Race-and-Sex-Analysis
Research Analysis of CHD and Race/Sex 

This research data is originally from my statistics class project, which utilizes a clinical dataset of 100 observations to investigate the primary demographic predictors of Coronary Heart Disease (CHD). Using Binomial Logistic Regression in jamovi, this analysis examines how variables such as Age, Sex, and Race influence the probability of a CHD diagnosis.

The goal of this project is to demonstrate competency in epidemiological data analysis, multivariate statistical modelling, and the interpretation of odds ratios (OR) in a public health context. 


With this dataset, I wanted to answer 2 questions: 
- Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? 

- Secondary: Is race also a significant factor for CHD? If so, which group is most prominent?




## 1) Primary: Is there evidence of higher CHD rates in males than in females, and vice versa? 

[Uploading CHD_M-F_<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        
        <title>Results</title>
        <style>

    body {
        font-family: "Segoe UI",Roboto,Helvetica,Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol" ;
        color: #333333 ;
        cursor: default ;
        margin: 24px;
        font-size: 12px ;
    }

    h1 {
        font-size: 160% ;
        color: #3E6DA9 ;
        margin-bottom: 12px ;
        white-space: nowrap ;
    }

    h2 {
        font-size: 130% ;
        margin-bottom: 12px ;
        color: #3E6DA9 ;
    }

    h3, h4, h5 {
        font-size: 110% ;
        margin-bottom: 12px ;
    }

    table {
        border-spacing: 0 ;
        page-break-inside: avoid;
    }

    table tr td, table tr th {
        page-break-inside: avoid;
        font-size: 12px ;
    }

    .ql-align-center {
        text-align: center;
    }

    .ql-align-right {
        text-align: right;
    }

    .ql-align-justify {
        text-align: justify;
    }

    .ql-indent-1 {
        padding-left: 3em;
    }

    .ql-indent-2 {
        padding-left: 6em;
    }

    .ql-indent-3 {
        padding-left: 9em;
    }

    .ql-indent-4 {
        padding-left: 12em;
    }

    .ql-indent-5 {
        padding-left: 15em;
    }

    .note {
        margin: 5px 0px;
    }
        </style>
</head>
<body>
    
                        <h1 contenteditable="" spellcheck="false" tabindex="-1">Results</h1>
                      
            
                <p style="text-align:left;padding:0px 0px 0px 0px;"></p>
            
        
            
            
        
                        <h1 contenteditable="" spellcheck="false" tabindex="-1">CHD Comparison of Male to Female</h1>
                      
            
                <p style="text-align:left;padding:0px 0px 0px 0px;"></p>
            
        <table aria-labelledby="5" tabindex="0"><thead><tr><th scope="colgroup" colspan="7" style="text-align:left;padding:4px 8px 4px 0px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:baseline;caption-side:top;"><span id="5" style="font-weight:400;">Model Fit Measures</span></th></tr></thead><thead><tr><th scope="colgroup" colspan="4" style="text-align:center;padding:4px 8px 4px 8px;border:0px;vertical-align:middle;"></th><th scope="colgroup" colspan="3" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Overall Model Test</th></tr><tr><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Model</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Deviance</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">AIC</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">R²<sub>McF</sub></th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">χ²</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">df</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">p</th></tr></thead><tbody><tr><td style="padding:8px 8px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">1<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">121.685<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">125.685<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">0.118<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">16.304<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">1<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">&lt;.001<span style="font-weight:400;"></span></td></tr></tbody><tfoot><tr><td colspan="7" style="padding:6px 8px 2px 8px;border:0px;vertical-align:middle;"><span style="font-style: italic ;" style="font-weight:400;">Note.</span> Models estimated using sample size of N=100</td></tr></tfoot></table><p>&nbsp;</p>
            
                <p style="text-align:left;padding:0px 0px 0px 0px;"></p>
            
        <table aria-labelledby="11" tabindex="0"><thead><tr><th scope="colgroup" colspan="10" style="text-align:left;padding:4px 8px 4px 0px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:baseline;caption-side:top;"><span id="11" style="font-weight:400;">Model Coefficients - CHD</span></th></tr></thead><thead><tr><th scope="colgroup" colspan="2" style="text-align:center;padding:4px 8px 4px 8px;border:0px;vertical-align:middle;"></th><th scope="colgroup" colspan="2" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">95% Confidence Interval</th><th scope="colgroup" colspan="4" style="text-align:center;padding:4px 8px 4px 8px;border:0px;vertical-align:middle;"></th><th scope="colgroup" colspan="2" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">95% Confidence Interval</th></tr><tr><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Predictor</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Estimate</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Lower</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Upper</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">SE</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Z</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">p</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Odds ratio</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Lower</th><th scope="col" style="text-align:center;padding:4px 8px 4px 8px;border-top:0px;border-right:0px;border-bottom:0.666667px solid rgb(51, 51, 51);border-left:0px;vertical-align:middle;">Upper</th></tr></thead><tbody><tr><td style="padding:8px 8px 2px 8px;border:0px;vertical-align:top;">Intercept<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">-0.999<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">-1.611<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">-0.386<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">0.313<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">-3.194<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">0.001<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">0.368<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">0.200<span style="font-weight:400;"></span></td><td style="text-align:right;padding:8px 20px 2px 8px;border:0px;vertical-align:top;">0.680<span style="font-weight:400;"></span></td></tr><tr><td style="padding:2px 8px 2px 8px;border:0px;vertical-align:top;">Sex:<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 2px 8px;border:0px;vertical-align:top;"> <span style="font-weight:400;"></span></td></tr><tr><td style="padding:2px 8px 8px 24px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">M – F<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">1.692<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">0.834<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">2.549<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">0.438<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">3.866<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">&lt;.001<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">5.429<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">2.302<span style="font-weight:400;"></span></td><td style="text-align:right;padding:2px 20px 8px 8px;border-top:0px;border-right:0px;border-bottom:2px solid rgb(51, 51, 51);border-left:0px;vertical-align:top;">12.799<span style="font-weight:400;"></span></td></tr></tbody><tfoot><tr><td colspan="10" style="padding:6px 8px 2px 8px;border:0px;vertical-align:middle;"><span style="font-style: italic ;" style="font-weight:400;">Note.</span> Estimates represent the log odds of &quot;CHD = 1&quot; vs. &quot;CHD = 0&quot;</td></tr></tfoot></table><p>&nbsp;</p>
            
                <p style="text-align:left;padding:0px 0px 0px 0px;"></p>
            
        
            
            
        
            
            
        
            
            
        
            
                <p style="text-align:left;padding:0px 0px 0px 0px;"></p>
            
        
            
            
        <h1 id="label-332">References</h1>
            
            <p data-checked="0" style="padding:2px 2px 2px 2px;">
                
                <span style="font-weight:700;">[1]</span>
                <span style="font-weight:400;">The jamovi project (2024). <em>jamovi</em>. (Version 2.6) [Computer Software]. Retrieved from <a href="https://www.jamovi.org" target="_blank">https://www.jamovi.org</a>.</span>
            </p>
        
            
            <p data-checked="0" style="padding:2px 2px 2px 2px;">
                
                <span style="font-weight:700;">[2]</span>
                <span style="font-weight:400;">R Core Team (2024). <em>R: A Language and environment for statistical computing</em>. (Version 4.4) [Computer software]. Retrieved from <a href="https://cran.r-project.org" target="_blank">https://cran.r-project.org</a>. (R packages retrieved from CRAN snapshot 2024-08-07).</span>
            </p>
        
</body>
</html>Analysis.html…]()



            


      



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
