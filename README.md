# Surfs_Up

## Overview

The purpose of this analysis is to use weather data to determine if Oahu is a good location for us to open up a surf and ice cream shop. Ideally, the location of our store is in a warm location without too much precipitation. In this project, we have a sqlite database of ~6 years' weather data for Oahu, then use Python and SQLAlchemy to parse and analyze the weather data. 

## Results

Overall, Oahu has relatively consistent temperatures year-round. In this analysis, we will use June and December as sample months to show two opposites of the year, which provides the ends of the spectrum we can expect in temperature over the course of a year. 

### June Temps
![image](https://user-images.githubusercontent.com/93338132/155861494-c3fff900-5048-4ef7-b471-d4de41d2187f.png)
![image](https://user-images.githubusercontent.com/93338132/155861496-2be468f4-52e9-4ddd-a700-dd0aa73977dc.png)

### December Temps
![image](https://user-images.githubusercontent.com/93338132/155861504-38cbe654-0988-4a69-bb98-4d5cdf7f9eb3.png)
![image](https://user-images.githubusercontent.com/93338132/155861509-d76259f9-bd06-4d31-80ce-5870fdfb7e7f.png)

### Comparison

* June has a higher avg temperature at 75 degrees F than December (71)
* December is slightly more variable in its temperatures with a Std Dev of 3.75 degrees F, vs June's 3.26
* December's IQR of temperatures is 5 vs June's 4 degrees and December has more outliers (see boxplots) despite fewer total readings ('count' in table)

## Summary
Overall, June is a warmer month with more consistent temperatures than December. However, December and June are both favorable temperatures for surfing and ice cream - each are warmer than 70 degrees on average.

There are a few more queries we could do to further solidify our recommendation to open the store here. First, we should run this same analysis for spring and fall time frames (March and Sept. as examples) to make sure we cover the 4 main seasons. We also should run this analysis with precipitation and wind speeds as variables, which are very impactful on surfing conditions. 

Last year's precipitation shown below for reference (in inches)
<img width="964" alt="image" src="https://user-images.githubusercontent.com/93338132/155861684-5c2fb1f2-dd83-4140-92ed-3e4ec7936a79.png">

