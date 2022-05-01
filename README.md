# Surf's Up Analysis
## Overview of Project
### Purpose

Based on W. Avy's weather data in SQLite database, we were able to provide more information about temperature trends to determine if the surf and ice cream shop business is sustainable year-round before opening the surf shop. This report will describe the key differences in weather between June and December and two recommendations for further analysis.

## Results

Using Python, Panda functions and methods, and SQLAlchemy, we filtered the date column of the Measurements table in the weather database to retrieve all the temperatures for the month of June and December. The generated summary statistics for June and December temperatures are presented in Figure 1.

![image](https://user-images.githubusercontent.com/99936542/166121629-a70f912a-d44b-4f82-abb4-ee51f35ddd84.png)
![image](https://user-images.githubusercontent.com/99936542/166121658-590d1156-ed6f-41d8-8089-b641645298fd.png)

<b>Fig.1 - June and December Temperatures Summary Statistics</b>

Based on the two analysis deliverables described above,

- There are 183 fewer temperature readings in December as there are in June.
- The average temperature in December is about 4&deg; colder than in June (71.04&deg; vs 74.94&deg; respectively). The standard deviation of the December temperatures is about 0.5&deg; higher than the standard deviation of the June temperatures, indicating that December temperatures are more spread out.
- The difference between the  minimum June and December temperatures is 8&deg; (56&deg; vs 64&deg; respectively) while the difference between the maximum June and December temperatures is 2&deg; (83&deg; vs 85&deg; respectively). 

## Summary

While the temperatures in June is very encouraging, there may be challenges associated with the increased variability and generally lower temperatures in December. However, the surf and ice cream shop business should be sustainable year-round overall since temperatures will most likely be above 70&deg; for majority of the year. 

Below are two additional queries that we could perform to gather more weather data:

1. Generate summary statistics for precipitation data for the months of June and December -- The lower the chance for precipitation, the more likely customers would like to spend their times outdoor.

![image](https://user-images.githubusercontent.com/99936542/166128061-c17d359c-57bc-4ad4-8e30-91c91f6e3030.png)

2. To understand the yearly weather patterns as a whole in Oahu, it would be beneificial to do similar temperature and precipitation analysis for the other months of the year as well.

## Resources
- Data Sources: hawaii.sqlite
- Software: Python 3.7.6, Jupyter Notebook 6.4.5