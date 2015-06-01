```stata
. use icu.dta

. logit STA AGE

Iteration 0:   log likelihood = -100.08048  
Iteration 1:   log likelihood = -96.261839  
Iteration 2:   log likelihood =  -96.15328  
Iteration 3:   log likelihood =  -96.15319  
Iteration 4:   log likelihood =  -96.15319  

Logistic regression                               Number of obs   =        200
                                                  LR chi2(1)      =       7.85
                                                  Prob > chi2     =     0.0051
Log likelihood =  -96.15319                       Pseudo R2       =     0.0392

------------------------------------------------------------------------------
         STA |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
         AGE |   .0275426   .0105647     2.61   0.009     .0068362     .048249
       _cons |  -3.058513    .696122    -4.39   0.000    -4.422887   -1.694139
------------------------------------------------------------------------------
```
```stata
. vce

Covariance matrix of coefficients of logit model

             | STA                    
        e(V) |        AGE       _cons 
-------------+------------------------
STA          |                        
         AGE |  .00011161             
       _cons | -.00710377   .48458582 
```
