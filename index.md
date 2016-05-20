---
title       : Developing Data Products Course Project
subtitle    : Prediction of Subject Reaction Time Based on
              Linear Analysis of Sleep Deprivation Data
author      : Gilbert Maerina
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- .class #id 
## Data 
Data are from the study described in Belenky et al. (2003), for the sleep-deprived group and for the first 10 days of the study, up to the recovery period. Data contains the average reaction time per day for subjects in a sleep deprivation study. The observations represent the average reaction time on a series of tests given each day to each subject.

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png)

---
## Prediction 

![plot of chunk smallplot](assets/fig/smallplot-1.png)

Through linear analysis, we can see that data is linear in nature. From this we develop a prediction function that is based on a linear model to develop an application that forecasts Reaction times based on Days inputted. 

---

## Cont.



```r
print(lmm$coeff)
```

```
## (Intercept)        Days 
##   251.40510    10.46729
```

As we can see, that the data increases by 251.4 msecs for every 10 days the subject(s) are deprived of sleep. Our application uses this simple linear model to predict the reaction time of of our subjects.

---

## Summary

### Thus using simple linear regression, we developed this application to predict Reaction time in milliseconds.

---
