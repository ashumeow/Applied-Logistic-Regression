```stata
. xi: logit STA AGE CAN CPR INF i.RACE
i.RACE            _IRACE_1-3          (naturally coded; _IRACE_1 omitted)

Iteration 0:   log likelihood = -100.08048  
Iteration 1:   log likelihood = -90.619912  
Iteration 2:   log likelihood = -89.663593  
Iteration 3:   log likelihood = -89.650384  
Iteration 4:   log likelihood = -89.650364  
Iteration 5:   log likelihood = -89.650364  

Logistic regression                               Number of obs   =        200
                                                  LR chi2(6)      =      20.86
                                                  Prob > chi2     =     0.0019
Log likelihood = -89.650364                       Pseudo R2       =     0.1042

------------------------------------------------------------------------------
         STA |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
         AGE |   .0271207   .0115879     2.34   0.019     .0044089    .0498325
         CAN |   .2445106   .6168152     0.40   0.692     -.964425    1.453446
         CPR |   1.646497   .6234137     2.64   0.008     .4246286    2.868365
         INF |   .6806676   .3804177     1.79   0.074    -.0649374    1.426273
    _IRACE_2 |  -.9570777   1.084474    -0.88   0.377    -3.082607    1.168452
    _IRACE_3 |   .2597493   .8712683     0.30   0.766    -1.447905    1.967404
       _cons |   -3.51152   .8144297    -4.31   0.000    -5.107773   -1.915267
------------------------------------------------------------------------------
```
```stata
. logit STA AGE CAN CPR INF

Iteration 0:   log likelihood = -100.08048  
Iteration 1:   log likelihood = -91.075007  
Iteration 2:   log likelihood = -90.210521  
Iteration 3:   log likelihood = -90.203821  
Iteration 4:   log likelihood =  -90.20382  

Logistic regression                               Number of obs   =        200
                                                  LR chi2(4)      =      19.75
                                                  Prob > chi2     =     0.0006
Log likelihood =  -90.20382                       Pseudo R2       =     0.0987

------------------------------------------------------------------------------
         STA |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
         AGE |   .0282536   .0114576     2.47   0.014     .0057971      .05071
         CAN |   .2015918   .6112054     0.33   0.742    -.9963488    1.399532
         CPR |   1.636655   .6155618     2.66   0.008      .430176    2.843134
         INF |   .7024685   .3779911     1.86   0.063    -.0383805    1.443318
       _cons |  -3.621061   .7902456    -4.58   0.000    -5.169914   -2.072208
------------------------------------------------------------------------------
```
```stata
. logit STA AGE CPR

Iteration 0:   log likelihood = -100.08048  
Iteration 1:   log likelihood = -92.714062  
Iteration 2:   log likelihood =  -91.98047  
Iteration 3:   log likelihood =  -91.97634  
Iteration 4:   log likelihood =  -91.97634  

Logistic regression                               Number of obs   =        200
                                                  LR chi2(2)      =      16.21
                                                  Prob > chi2     =     0.0003
Log likelihood =  -91.97634                       Pseudo R2       =     0.0810

------------------------------------------------------------------------------
         STA |      Coef.   Std. Err.      z    P>|z|     [95% Conf. Interval]
-------------+----------------------------------------------------------------
         AGE |   .0296074   .0111489     2.66   0.008     .0077559    .0514589
         CPR |   1.784092   .6072971     2.94   0.003     .5938115    2.974373
       _cons |  -3.351955   .7454995    -4.50   0.000    -4.813108   -1.890803
------------------------------------------------------------------------------
```
