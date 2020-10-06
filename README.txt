# Hadoop_Project_5
#HIVE
This is a historical dataset on the modern Olympic Games, including all the Games from Athens 1896 to Rio 2016. I scraped this data from www.sports-reference.com in May 2018. The HIVE code I used to scrape and wrangle the data is on GitHub. 

Noting that the Winter and Summer Games were held in the same year up until 1992. After that, they staggered them such that Winter Games occur on a four year cycle starting with 1994, then Summer in 1996, then Winter in 1998, and so on.

The file athlete_events.csv contains 271116 rows and 15 columns. Each row corresponds to an individual athlete competing in an individual Olympic event (athlete-events). The columns are:

ID - Unique number for each athlete
Name - Athlete's name
Sex - M or F
Age - Integer
Height - In centimeters
Weight - In kilograms
Team - Team name
NOC - National Olympic Committee 3-letter code
Games - Year and season
Year - Integer
Season - Summer or Winter
City - Host city
Sport - Sport
Event - Event
Medal - Gold, Silver, Bronze, or NA

Our Inspiration
We have viewed www.randigriffin.com on kaggle as well for his data scrapping part. Thank you!

#PIG
A basic analysis of daily-temperature data of Mumbai city obtained from-
https://academic.udayton.edu/kissock/http/Weather/gsod95-current/INBOMBAY.txt

The data is in the format
[month, day, year, average temperature].

Average temperature is the average of Low/High Temperature issued by the weather station in Colaba, Mumbai.

We're using basic Apache-PIG commands such as 
LOAD
FILTER
FOREACH
GENERATE
GROUPED
SPLIT
AVG
MIN
MAX
COUNT.

On a very crude level, this analysis is trying to find out which days stand out when daily temperature is compared to the average of the season to which the day belongs.

With a bigger dataset and more variables to support further analysis, we could determine why these days stand out which will have a great future impact in Weather forecasting.
