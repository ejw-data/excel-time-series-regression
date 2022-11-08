# excel-time-series-regression

Author:  Erin James Wills, ejw.data@gmail.com  

![Regression](./images/time-series-regression.png)  

<br>

## Overview  
<hr>  
Example showcasing how to incorporate time dependent data into a multiregression.

<br>

## Analysis
*  Dataset generated works well.  The dataset should have a very high R<sup>2</sup>.  Since the dataset is designed to include time series, by dedimensionalizing the time series the linear fit goes up a bit - from 0.99 to 0.9999. 

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