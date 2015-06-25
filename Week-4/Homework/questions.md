```
Exercise One

For this exercise, 
you will use the ICU dataset. 
You can download the icu.dta Stata file, 
or you can also access the data through this CSV file.


Complete the following:

Consider the ICU data and use as the outcome variable vital status (STA) and race (RACE) as a covariate. 
Prepare a table showing the coding of the two design variables for RACE using the value RACE = 1, white, as the reference group.

Show that the estimated log-odds ratios obtained from the cross-classification of STA by RACE, using RACE = 1 as the reference group, are identical to estimated slope coefficients for the two design variables from the logistic regression of STA on RACE.

Verify that the estimated standard errors of the estimated slope coefficients for the two design variables for RACE are identical to the square root of the sum of the inverse of the cell frequencies from the cross-classification of STA by RACE used to calculate the odds ratio.

Use either set of computations to compute the 95% Confidence Interval for the odds ratios.
```
```
Exercise Two

For this exercise, 
you will continue using the ICU dataset.


Complete the following:

Create design variables for RACE using the method typically employed in ANOVA.

Perform the logistic regression of STA on RACE.

Show by calculation that the estimated logit differences of RACE = 2 versus RACE = 1 and RACE = 3 versus RACE = 1 are equivalent to the values of the log-odds ratio obtained in exercise 1.

Use the results of the logistic regression to obtain the 95% Confidence Interval for the odds ratios and verify that they are the same limits as obtained in exercise 1. 
Note that the estimated covariance matrix for the estimated coefficients is needed to obtain the estimated variances of the logit differences.
```