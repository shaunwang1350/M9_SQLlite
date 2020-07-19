# M9_SQLite_Challenge

### Objectives
The goals of this challenge are to:

* Determine key statistical data about the month of June.
* Determine key statistical data about the month of December.
* Compare your findings between the month of June and December.
* Make 2 or 3 recommendations for further analysis.
* Share your findings in the Jupyter Notebook.

### Procedure
Completed the following steps.
1. Identifing key statistical data in June across all of the stations and years using the describe() function.
    1. Set date range using dt.date(), and creating an empty list to save results.
    2. Looping through data, which increments by each for reach iteration.
    3. Querying temperature and participation and is groupby by date for the month of June. This allows for the inclusion of all stations.
    4. Porting the data into a dataframe, and then taking the descriptive data of each dataframe.

2. Identifing key statistical data in December across all of the stations and years using the describe() function.
    1. Set date range using dt.date(), and creating an empty list to save results.
    2. Looping through data, which increments by each for reach iteration.
    3. Querying temperature and participation and is groupby by date for the month of December. This allows for the inclusion of all stations.
    4. Porting the data into a dataframe, and then taking the descriptive data of each dataframe.

3. Comparing findings between the month of June and December
    1. Creating dataframes to compare the precipitation / temperature for june and december.
    2. Added a new column to show the difference between the two months.

### Troubles:
During the process there were a few problems that I ran into:
* The most tricky problem is that if one used a while loop and incremented time using .timedelta, there would be miscalculation in data, since there are leap years involved. This meant that the dates for the data would be off by 2 days by the end of 2017.
* There are also no december 2017 data for either temperature or precipitation. This meant that the count for individual dates will be slightly off.     

### Recommendations for further Analysis
#### Recommendation 1:
Comparing the mean and std for precipitation across the two months, there seems to be a huge difference, where december's mean and std is roughly 50% higher than that of june. This is also true when comparing the max of the the two months, where june's max precipitation is nearly twice as high as that of december. 

Precipitation has to do with things falling down, and not just from the sky, and is expressed in percentages. What this means is that the months of December has a much higher likelihood of raining that of June. 

In other words, Oahu’s has a high variability of raining within the month of december. Since people are less likely to eat icecream when its raining, I would advise that there are plans to circumvent possible top-line reductions due to december weather patterns. That said, rainy weather also allows for bigger waves, meaning that the daredevil surfers would be more likely to surf. 

#### Recommendation 2:
The changes in weather temperature is much less between the months of June and December. The mean difference is around 6 degrees fahrenheit. While it is still change, there won't be a drastic change where customers will havea shift in clothing or feel uncomfortable on the beach. 

However, looking at the min and std for the month of December. December's std is twice that of june and that the min temperature can be 56, which means that there will be cold days, where customers wouldn't want icecream to go surfing. 

In other words, while the average mean temperature isn't too much of a shift between the two months. The variability of the month of december will have an effect on the top-line for the month of december. 

### Possible Future Analysis:
* I would recommend doing creating an descriptive analysis on all months of the year. This way it will inform when the business should heavily supply itself on icecream and surf equipment. In other words, the surf/icecream will become a seasonal business rather than an all year round business.
* If the shop owner intends to open the shop all year round, I would recommend to invest in alternative business plans during days where it is raining or is too cold to swim. A future analysis would include investigating what are popular businesses during the time when it is raining or too cold to surf on the beach. 