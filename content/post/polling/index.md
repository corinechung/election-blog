---
title: Polling
author: ''
date: ''
slug: []
categories: []
tags: []
---

# Comparing Midterm Forecasts

** FiveThirtyEight Model 

FiveThirtyEight utilizes three different versions of models: Lite, Classic, and Deluxe. These versions, however, can be considered to be layers that build on top of one another. For instance, the Lite version incorporates district-by-district polling (adjusted for house effects and other factors) and CANTOR, which is a system that infers results for districts with little or no polling from comparable districts that do have polling data available. The next version, Classic, includes all of the aspects of the Lite version, while also implementing fundamentals, or non-polling factors such as fundraising, incumbency, and past election results that historically have helped in predicting congressional races. Finally, the Deluxe version includes all of the aforementioned layers while adding expert forecasts, which are ratings of each race published by the Cook Political Report, Inside Elections, and Sabato's Crystal Ball. 

FiveThirtyEight also takes into account a variety of other factors. When collecting polls, FiveThirtyEight also includes partisan polls, but ensures that the polls they gather meet some criteria. For instance, they will not use polls that have a significant concern about the veracity nor will they use polls that have been commissioned by nonprofessional hobbyists. 

Polls are also weighted based on the sample size, the recency, and their pollster rating. There are also three adjustments made to each poll: a likely voter adjustment, a timeline adjustment, and a house effects adjustment. Moreover, FiveThirtyEight's model accounts for the possibility of a uniform national swing, which is when the polls are systematically favoring one party's direction in almost every race. 

** Economist Model

The Economist seems to use some similar approaches that FiveThirtyEight uses. For example, the Economist also has models to assess fundamentals, which include previous election results and campaign contributions.

However, one main difference is that the Economist seems to place more of an emphasis on the generic ballot as opposed to a variety of polling measures that is used by FiveThirtyEight. Besides using fundamentals to build on this model, the Economist also takes into account the popularity of the president and partisan lean when determining their voting-based predictors. 

After examining the political climate on a national level, the Economist then looks at district-level data. For each district, there are two considerations: voting history and information about the candidates. Then, two nationwide factors are added: the share of swing voters in the electorate and observed, adjusted national popular vote. One additional consideration is that given district-level votes do not follow a normal distribution, the Economist uses a skew-T distribution. 

** Conclusion

Though I believe that both methods have their merits, I believe that the Economist's method is more precise because it emphasizes the generic ballot more so than local polling, which may be subject to more bias and variation. FiveThirtyEight says that they use partisan polls, which are a "necessary evil," since there is no way to avoid them for the House. Though I wonder if FiveThirtyEight has a way of weighing their polls based on pollster ratings. 


# Poll Variations





First I examine the variations in polls. As we saw, FiveThirtyEight has a detailed ranking of specific polling agencies and their respective polls. To better understand poll variation, I examine the proportion of races called correctly for all of the pollsters that have been ranked by FiveThirtyEight. 

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-3-1.png" width="672" />
I do the same for the proportion of missed races outside of each pollster's margin of error. 

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-4-1.png" width="672" />

I was pleased to find that for the races called correctly, most polls were in the category where between 90% and 100% of polls were called correctly and that for the misses outside the margin of error, most polls were in the category where there were between 0% and 10% of misses outside the MOE. However, I was surprised to see about 70 polls had between 90% and 100% misses. Another nuance to consider is that some pollster have only conducted one or two polls while others have conducted dozens. Perhaps putting a weight on the races called correctly or misses outside the MOE would be a better approach when comparing pollsters that have conducted varying numbers of polls.

# 2018 and 2022 Generic Polls: State Level





Next, I examine the 2018 and 2022 generic ballots for two key swing-states: Michigan and Pennsylvania.

Here, I look at the 2018 and 2022 generic ballot support for Michigan and how support changes throughout the year. The x-axis is weeks of each year, starting on the first Sunday. 

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-7-1.png" width="672" />





<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-10-1.png" width="672" />

Here is the 2018 and 2022 generic ballot support and their fluctuations throughout the year for Pennsylvania.

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-11-1.png" width="672" />

<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-12-1.png" width="672" />

Similar to the model we examined in section, which looked at generic ballot support in 2018 on a national level, generic ballot support within states fluctuates across times. However, one difference is that because of less polling data, sometimes this fluctuation is more difficult to gage.
