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
  