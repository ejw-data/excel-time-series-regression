# excel-time-series-regression

Author:  Erin James Wills, ejw.data@gmail.com  

![Regression](./images/time-series-regression.png)  
<cite>Photo by [Jack B](https://unsplash.com/@nervum?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/stock-market?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)</cite> 

<br>

## Overview  
<hr>  
Example showcasing how to incorporate time dependent data into a multiregression.

<br>

## Analysis
*  Dataset generated works well.  The dataset should have a very high R<sup>2</sup>.  Since the dataset is designed to include time series, by dedimensionalizing the time series the linear fit goes up a bit - from 0.99 to 0.9999.  

*  The time series feature of the dataset is the outside temperature measurement.  To make the the energy usage of the home dependent on the historical measurement of the temperature, the average temperature across three hours was used to calculate the heat flux of the house with a standard internal house temperature of 73<sup>o</sup>F.  To account for these historical influences, three features representing the heat flux were created - 1) flux 2 hours before, 2) flux 1 hour before, and 3) the current heat flux of the current hour.  Each feature was modeled as a historical trend for each record.  

## Next Stages
1.  Add randomness into the dataset features and test regression models.
1.  Add features that are dependent on other features (slight dependencies)
1.  Transform features by different methods and retest regression
    - Use temperature instead of heat load
    - Test effects of using Kelvin, Celsius, Fahrenheit
    - Should a temperature reference point be used?  This might not be known for all cases.  I used 73<sup>o</sup>F aka 21.7<sup>o</sup>C as a common reference point.  How can I get around this background knowledge?  
    - what if I bin square footage to be labels instead of values?  What effect does this have on the accuracy.  
1.  Add features
    - Daylight/Night time
    - Cloudiness
    - Wind Speed  
    - Is seasonality needed?



## Technologies    
*  Excel
*  Stats Toolkit Add-on

## References  

1.  https://constructionphysics.substack.com/p/looking-at-energy-use-in-us-residential  
<br>