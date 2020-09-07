# surfs_up
## Purpose and Background
This analysis is follow-on analysis to an initial weather analysis conducted previously. The overall goal is to determine if opening a shake and surf
shop on Oahu makes good financial sense due to weather conditions. Initial analysis revealed it does make good sense and the weather
is conducive to this type of business. The investor, W. Avy, had a follow up question. He wants to understand what the weather is like for
the months of June and December. This analysis answers that question.

## Overview of Analysis
The data to conduct this analysis is a data set supplied by W. Avy in a SQL Lite file. The pertinent part for this analysis contains dates and temperatures but percipitation is also available for Oahu from 01/01/2010 through 08/23/2017.

The data was brought into a Jupyter notebook and using python, and sqlalchemy along with Numpy and Pandas the analysis was conducted.

### Analysis Steps
The specific analysis steps conducted were:
1.	created a query using sqlalchemy to first understand the data. In addition to the dates, listed above, the data contains 19,550 rows and 2 columns, date and temperatures (tobs).
2. Focusing on June, a query was written to view the dates and temperatures for the month of June. These are all the temperatures from 2010 through 2017, 1700 rows.
3. The June data was put into a list and then into a dataframe.
4. Using the describe function you can see the results here ![](https://github.com/davidmcbee/surfs_up/blob/master/Resources/june_statistics.png)

Figure 1


5. Now, focusing on December, a query was written to view the dates and temperatures for the month of December. These are all the temperatures from 2010 through 2016, the data only goes through 08/23/2017 so no temperatures are available for 2017. This resulted in 1517 rows.
3. The December data was put into a list and then into a dataframe.
4. Using the describe function you can see the results here ![](https://github.com/davidmcbee/surfs_up/blob/master/Resources/december_statistics.png)

Figure 2

## Results

### June
To answer the question of how weather for June and December will effect business the following is provided.
1. For June, the mean temperature is 74.9 degrees. This is nice weather
2. For June, the standard deviation is 3.26. This means the temperature will normally not go lower then 71.68.
3. For June, the median is 75. This means that for the 1700 measurements half were above 75 and half were below 75.
4. For June, the maximum temperature recorded was 85 degrees.

Overall, June is very temperate

### December
1. For December, the mean temperature is 71 degrees. This is also nice weather
2. For December, the standard deviation is 3.75. This mans the temperature will normally not go lower then 67.25.
3. For December, the median is 71. This means that for the 1517 measurements half were above 71 and half were below 71.
4. For December, the maximum temperature recorded was 83 degrees.
 
Overall, December is also very temperate but on average, 3.9 degrees colder than June. This could negatively effect shake sales. Perhaps offering hot cocoa in December would help.

### Additional Information
The other factor that could affect sales is rain. To understand this for June and December see figures 3 and 4 below
Notice that the mean amount of precipitation for June is .136 inches and for December is .2168 inches. This is very light.
Also, with the standard deviations of .336 and .541 inches for June and December respectively, the most it will normally rain is .47 inches in June and .76 inches in December.
Having said that sometimes it doe rain rather heavily. This can be seen in the maximum values of 4.43 inches in June and 6.42 inches in December
The hot cocoa along with a covered patio would help when these heavy rains do occur

![](https://github.com/davidmcbee/surfs_up/blob/master/Resources/june_rain.png)

Figure 3

![](https://github.com/davidmcbee/surfs_up/blob/master/Resources/december_rain.png)

Figure 4
