---
title: Economic Forces
author: ''
date: ''
slug: []
categories: []
tags: []
---


*This blog is part of a series related to Gov 1347: Election Analytics, a course at [Harvard University](https://www.harvard.edu/) taught by Professor [Ryan D. Enos](http://ryandenos.com/)*.

<br>

From now until November 8, I will be updating this weekly blog series with my **2022 US midterm election prediction model**. For this second blog, I explore national economic models as predictors for the incumbent party's popular vote percentage in a given election year.

<br>

# Real Disposable Income Quarterly

<br> 

First, I examine the percent change in disposable income and how that correlates with the percentage of the votes that the incumbent party receives for each election year from 1964 to 2020.

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-1-1.png" width="60%" style="display: block; margin: auto;" />
We can see that for most of the time, a positive percent change in disposable income results in the incumbent party receiving more votes.

<br>

The correlation is found to be:






```
## 
## Call:
## lm(formula = H_incumbent_party_majorvote_pct ~ DSPIC_change_pct, 
##     data = data2)
## 
## Residuals:
##     Min      1Q  Median      3Q     Max 
## -6.3857 -2.1887  0.4447  2.2152  5.8840 
## 
## Coefficients:
##                  Estimate Std. Error t value Pr(>|t|)    
## (Intercept)       52.5781     0.7597  69.210   <2e-16 ***
## DSPIC_change_pct  -0.7964     0.6085  -1.309    0.201    
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 3.4 on 29 degrees of freedom
## Multiple R-squared:  0.05577,	Adjusted R-squared:  0.02321 
## F-statistic: 1.713 on 1 and 29 DF,  p-value: 0.2009
```


```
## [1] 0.05576812
```

The following graph shows the incumbent party vote percentage when compared to the predicted incumbent party vote percentage for each year:

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-6-1.png" width="70%" style="display: block; margin: auto;" />



Below is the mean out-of-sample residuals, which validates our model:

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-8-1.png" width="70%" style="display: block; margin: auto;" />

```
## [1] 1.159056
```

Next, I examine the percent change in unemployment rate and how that correlates with the percentage of the votes that the incumbent party receives for each election year from 1964 to 2020.

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-10-1.png" width="60%" style="display: block; margin: auto;" />
There does not seem to be a strong correlation between unemployment rate and the percentage of votes the incumbent party receives. This model seems to go against intuition, since one would suppose that more unemployment would cause constituents to be unhappy with the current government.

<br>

The correlation is found to be:






```
## 
## Call:
## lm(formula = H_incumbent_party_majorvote_pct ~ UNRATE, data = data3)
## 
## Residuals:
##     Min      1Q  Median      3Q     Max 
## -7.9681 -1.4497  0.6175  2.3157  6.6103 
## 
## Coefficients:
##             Estimate Std. Error t value Pr(>|t|)    
## (Intercept)  47.4800     1.9400  24.475   <2e-16 ***
## UNRATE        0.7466     0.3254   2.294   0.0279 *  
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 3.18 on 35 degrees of freedom
## Multiple R-squared:  0.1307,	Adjusted R-squared:  0.1059 
## F-statistic: 5.263 on 1 and 35 DF,  p-value: 0.0279
```


```
## [1] 0.1307167
```

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-15-1.png" width="70%" style="display: block; margin: auto;" />



Below is the mean out-of-sample residuals:

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-17-1.png" width="70%" style="display: block; margin: auto;" />

```
## [1] 1.084569
```
