```
For this exercise, 
you will use the ICU Study dataset. 

If you need the file you can download the icu.dta Stata file, or you can also access the data through the CSV file.


First, using the ICU data, consider the multiple logistic regression model of vital status, STA, on age (AGE), cancer part of the present problem (CAN), CPR prior to ICU admission (CPR), infection probable at ICU admission (INF), and race (RACE).

Then, complete the following:

The variable RACE is coded at three levels. 
Prepare a table showing the coding of the two design variables necessary for including this variable in a logistic regression model.
Write down the equation for the logistic regression model of STA on AGE, CAN, CPR, INF, and RACE. 
Write down the equation for the logit transformation of this logistic regression model. 
How many parameters does this model contain?
Write down an expression for the likelihood and log likelihood for the logistic regression model in part (b). 
How many likelihood equations are there? Write down an expression for a typical likelihood equation for this problem.

Using a logistic regression package, 
obtain the maximum likelihood estimates of the parameters of the logistic regression model in part (b). 
Using these estimates write down the equation for the fitted values, that is, the estimated logistic probabilities.

Using the results of the output from the logistic regression package used in part (d), 
assess the significance of the slope coefficients for the variables in the model using the likelihood ratio test. 

What assumptions are needed for the p-values computed for this test to be valid? 
What is the value of the deviance for the fitted model?
Use the Wald statistics to obtain an approximation to the significance of the individual slope coefficients for the variables in the model. 
Fit a reduced model that eliminates those variables with nonsignificant Wald statistics. 
Assess the joint (conditional) significance of the variables excluded from the model. 
Present the results of fitting the reduced model in a table.

Using the results from part (f), 
compute 95 percent confidence intervals for all coefficients in the model. 

Write a sentence interpreting the confidence intervals for the non-constant covariates.
You can share your response and discuss this exercise in the homework forum.
```
