# Surfs Up Challenge

## Overview

Opening a new business is not as simple as just having a good idea and executing well. The location of the business can be cause even the most brilliant businesses to fail. In this analysis, we are looking at opening a surf and ice cream shop in Hawaii. It makes sense that more people would be willing to spend money on these items on good weather days, and that business would be quite slow on rainy days.

This is exactly the experience that our investor encountered when opening a similar shop. In order to avoid these pitfalls, we gathered some weather data from public data via sqlite and are looking at the statistaical patterns in the data to help our investor decide to invest. We've picked June and December in order to presumably look at the best and worst months for business. 

## Analysis

### Results of Analysis: Tables

Here are the two tables showing the weather stats for June and December. Given the count of data points being over 1500 in each table, these results are likely statistically relevant

![June](https://user-images.githubusercontent.com/109319148/192055277-b758bed6-b070-40be-a58e-c26dc60f7123.png)

![December](https://user-images.githubusercontent.com/109319148/192055295-97d69811-3e03-487d-8774-8bd4c977f876.png)

### Analysis of Tables

  * The temperature in this location seems to be pretty consistent. The average temperature in December is only 4 degrees cooler than in June. It seems that by looking at averages, the weather remains pretty comfortable all year round.

  * The standard deviation in temperatures is also relatively close between June and December. June has a standard deviation of 3.25 and December is only a half a degree different at 3.75. We can infer that there are not wild temperature swings from day day. Just looking at an average, it could be misleading because it might be made up of very high and very low numbers. The standard deviation less than 4 degrees tells us that the max and the min are probably not extremely far from the average

  * The interquartile ratios of month are also closely clustered in the low-mid 70 degree ranges. This suggests that this is pleasant weather that is neither too hot or too cold for at least half the month. The upper bounds don't exceed the mid 80s for either month, with the lower bounds falling to mid 50s in December. Given that less than 25% of days in December were below 69 degrees, this is a good sign that the temperature is pleasant most days.

## Summary
  
  If we are only looking at temperature, then the results of our analysis are favorable for this location. The temperature is neither too hot or too cold an does not vary drastically from the mean. We have a decent amount of data points to make this decision based on temperature. Our quartile analysis gives us even more confidence that most days are temperate in the 70's and conducive to a business catered to warm weather. 
  
  In earlier analysis we looked at precipitation and now we've looked at temperature. These are both incredibly important, but the next query should be done on a data table containing information on wind speed. This is going to help us decide if there are ideal surf conditions near the shop. Wind is the most important thing to consider when looking at surf conditions. If the wind is not as ideal as we'd like, we probably need to think about making the ice cream part of the business bigger in order to maintain cash flow. We might also add other services such as surf board detailing or repair or offer paddleboards that don't need wind. Filtering this query by station location is important since the wind needs to be from off-shore stations if they exist. Off-shore wind is preferable to on-shore wind. Too much wind makes surfing conditions challenging
  
  Another important thing to query is data about the tides. This is going to help us understand business hours and if they are going to vary drastically in the winter from the summer. We want to understand when the surfers are going to be in the water and when we we would like to lure them to our shop. Hawaii is closer to the equator than New York, so we can speculate that these also do not vary drastically. We could also look at swell size if there is data available. 
  
  A few additional queries would help our investor not only decide if this is the right location, but also how to position the business for success. 
  
  

