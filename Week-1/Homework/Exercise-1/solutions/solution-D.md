``` stata
. use MYOPIA.dta

. sum

    Variable |       Obs        Mean    Std. Dev.       Min        Max
-------------+--------------------------------------------------------
          ID |       618       309.5    178.5455          1        618
   STUDYYEAR |       618    1992.359    1.734507       1990       1995
      MYOPIC |       618     .131068     .337748          0          1
         AGE |       618    6.299353    .7129501          5          9
      GENDER |       618    .4886731    .5002766          0          1
-------------+--------------------------------------------------------
       SPHEQ |       618    .8010097    .6259184      -.699      4.372
          AL |       618    22.49678    .6801414       19.9      24.56
         ACD |       618    3.578629    .2303938      2.772       4.25
          LT |       618    3.541453    .1545192       2.96      4.112
         VCD |       618    15.37678    .6641831      13.38       17.3
-------------+--------------------------------------------------------
     SPORTHR |       618    11.95307    7.968296          0         45
      READHR |       618    2.796117    3.068191          0         20
      COMPHR |       618    2.105178    3.056508          0         30
     STUDYHR |       618    1.490291    2.216207          0         15
        TVHR |       618     8.94822    5.719021          0         31
-------------+--------------------------------------------------------
   DIOPTERHR |       618     26.0178    16.03172          2        101
       MOMMY |       618    .5064725    .5003631          0          1
       DADMY |       618    .4983819    .5004024          0          1

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

. predict p
(option pr assumed; Pr(MYOPIC))

. twoway(scatter MYOPIC SPHEQ) (scatter p SPHEQ)

. graph export "D:\Graph1.png", as(png) replace
(note: file D:\Graph1.png not found)
(file D:\Graph1.png written in PNG format)
```
![](http://geekresearchlab.net/coursera/applied-log-regress/Graph1.png)
