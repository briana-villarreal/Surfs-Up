# Surfs-Up
## Overview of the Project
### Purpose
A new shop idea for Oahu Island, Surf n’ Shake, needs investor backing. My client, W. Avy, is interested in determining if this business idea is sustainable year-round. To determine sustainability, I conducted an analysis on the weather trends in Oahu. Specifically, I examined temperature data for the months of June and December.
## Results
### Major Points
* To analyze temperature patterns for June, I wrote a query that filtered the date column from the Measurement table to retrieve all the temperatures for the month. To get June as the specific month, I utilized the extract method and conditionals. I then used list comprehension to convert the June temperatures to a list. I created a dataframe, named June_df, using the pd.DataFrame() function. I named the columns "June Temperatures". I then generated the summary statistics for the June temperatures DataFrame using the describe() method. 
![june 1](https://user-images.githubusercontent.com/106560739/183791393-c3477653-48ba-417d-98ad-43a426687f02.png)
![jun sum](https://user-images.githubusercontent.com/106560739/183791400-7d87a940-0e42-4583-8326-9addf2637ba9.png)
Upon calculating the summary statistics, I found that the highest temperature recorded out of the 1700 data points for the month of June was 85.00 degrees Fahrenheit. The lowest temperature recorded in June was 64.00 degrees Fahrenheit. 
* To analyze temperature patterns for December, I wrote a query that filtered the date column from the Measurement table to retrieve all the temperatures for the month. To get December as the specific month, I utilized the extract method and conditionals. I then used list comprehension to convert the December temperatures to a list. I created a dataframe, named Dec_df, using the pd.DataFrame() function. I named the columns "December Temperatures". I then generated the summary statistics for the December temperatures DataFrame using the describe() method. 
![dec 1](https://user-images.githubusercontent.com/106560739/183791432-cc4368ab-ab51-4c7e-be17-188eaf1484b3.png)
![dec sum](https://user-images.githubusercontent.com/106560739/183791437-7a0a9349-a0d2-49a3-8788-25f606633d97.png)
Upon calculating the summary statistics, I found that the highest temperature recorded out of the 1517 data points for the month of December was 83.00 degrees Fahrenheit. The lowest temperature recorded in December was 56.00 degrees Fahrenheit. 
* Upon comparing the summary statistics for both months, I found that the temperature for June is on average higher than December. The mean or average temperature in June is approximately 74.94 degrees Fahrenheit. This contrasts with December as the mean or average temperature during this month is approximately 71.04 degrees Fahrenheit.
## Summary
### Additional Insights
The temperature in Oahu is fairly consistent year-round as evidenced by similar average temperatures for the months of June and December. There is approximately a 3.9 degrees Fahrenheit difference between these two months. Therefore, based on my analysis, the new shop idea seems sustainable year-round. However, gathering more weather data would help guarantee sustainability. There are two additional queries I would perform to gather more weather data for June and December. The first query I recommend conducting is one to retrieve precipitation data for the two months. I would perform a query that filtered the date column from the Measurement table to retrieve precipitation data for the two months. I would employ the extract method and conditionals to specify the month. I then would use list comprehension to convert the June and December precipitation results to a list. I would create a dataframe for each month and generate summary statistics using the describe() method on each dataframe. The second query I recommend conducting is one to retrieve station data. I would write a query that determines the most active weather stations from the Measurement table. I would use the func.count() operator and the group_by() method on "Measurement.station" to obtain the most active. Overall both of these queries would aid the shop in maintaining sustainable business. The precipitation query would allow the shop to determine precipitation levels throuhgout the year. The station query would allow the shop to rely on the most active stations for weather updates and information.
