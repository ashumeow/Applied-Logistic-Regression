```
For this exercise, you will use the Hyponatremia dataset (this is the same data from week 4). 
You can download the hyponatremia.dta Stata file, or you can also access the data through this CSV file.

If you recall from last week, 
the data for this homework exercise derive from an epidemiological study of hyponatremia (a life-threatening condition) among runners of the 2002 Boston Marathon. 
Hyponatremia is defined as an electrolyte disturbance in which the serum sodium concentration is lower than normal (<135 mmol/l).
```
```
Complete the following:

Assess the association between hyponatremia (dichotomous variable nas135) and sex (variable female) by making a 2 by 2 table. 
Calculate the odds ratio of hyponatremia of a female compared to a male. 
Compute the 95% confidence interval for this odds ratio. Interpret the findings.

Perform a logistic regression analysis with Stata using nas135 as dependent variable and female as the only independent variable. 
Use the Likelihood Ratio test to assess the significance of the model. 
Is the model with female a better model than the naïve model? 

If you are using Stata, you can use their built-in statistical functions to obtain p-values (type help functions).

What is the naïve model? What is the probability of hyponatremia that this model predicts?

Run a logistic regression analyses with no independent variables. 
Transform the coefficient obtained from this model into a probability.

Using the model with female as independent variable, 
compute the estimated probability of hyponatremia per males and females. 
Write down the equation for the logit.

Use the Wald test to assess the significance of the coefficient for female.

Fit a model with runtime as the only independent variable. Assess the significance of the model.

Calculate the probability of hyponatremia of a runner who takes 4 hours (240 minutes) to complete the marathon.

Fit a model with female and runtime as independent variables. 
Assess the significance of the model. 
Which null hypothesis is tested?
```
