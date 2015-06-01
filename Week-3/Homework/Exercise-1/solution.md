```stata
. use MYOPIA.dta

. logit MYOPIC SPHEQ

Iteration 0:   log likelihood = -240.03851  
Iteration 1:   log likelihood = -185.66235  
Iteration 2:   log likelihood = -168.99543  
Iteration 3:   log likelihood = -168.67355  
Iteration 4:   log likelihood = -168.67244  
Iteration 5:   log likelihood = -168.67244  

Logistic regression                               Number of obs   =        618
                                                  LR chi2(1)      =     142.73
                                                  Prob > chi2     =     0.0000
Log likelihood = -168.67244                       Pseudo R2       =     0.2973

------------------------------------------------------------------------------
      MYOPIC |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
       SPHEQ |  -3.833098   .4183899    -9.16   0.000    -4.653127   -3.013068
       _cons |   .0539731    .206752     0.26   0.794    -.3512533    .4591996
------------------------------------------------------------------------------
```
```stata
. vce

Covariance matrix of coefficients of logit model

             | MYOPIC                 
        e(V) |      SPHEQ       _cons 
-------------+------------------------
MYOPIC       |                        
       SPHEQ |  .17505013             
       _cons | -.06338157   .04274638 
```
```stata
. lincom _b[_cons]+_b[SPHEQ]*2

 ( 1)  2*[MYOPIC]SPHEQ + [MYOPIC]_cons = 0

------------------------------------------------------------------------------
      MYOPIC |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
         (1) |  -7.612222    .699586   -10.88   0.000    -8.983385   -6.241059
------------------------------------------------------------------------------
```
```stata
. adjust SPHEQ=2, pr ci

-------------------------------------------------------------------------------
     Dependent variable: MYOPIC     Equation: MYOPIC     Command: logit
 Covariate set to value: SPHEQ = 2
-------------------------------------------------------------------------------

----------------------------------------------
      All |         pr          lb          ub
----------+-----------------------------------
          |    .000494    [.000125    .001944]
----------------------------------------------
     Key:  pr         =  Probability
           [lb , ub]  =  [95% Confidence Interval]
```
