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
. estimates store A

. quietly logit MYOPIC

. lrtest A

Likelihood-ratio test                                 LR chi2(1)  =    142.73
(Assumption: . nested in A)                           Prob > chi2 =    0.0000

. logistic MYOPIC SPHEQ

Logistic regression                               Number of obs   =        618
                                                  LR chi2(1)      =     142.73
                                                  Prob > chi2     =     0.0000
Log likelihood = -168.67244                       Pseudo R2       =     0.2973

------------------------------------------------------------------------------
      MYOPIC | Odds Ratio   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
       SPHEQ |   .0216425    .009055    -9.16   0.000     .0095318    .0491407
       _cons |   1.055456   .2182177     0.26   0.794     .7038055    1.582807
------------------------------------------------------------------------------
```
