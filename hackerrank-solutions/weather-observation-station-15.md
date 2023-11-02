## Weather Observation Station 15

Query the Western Longitude (LONG_W) for the largest Northern Latitude (LAT_N) in STATION that is less than 137.2345. Round your answer to 4 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT ROUND(long_w, 4)
FROM station
WHERE lat_n = 
    (SELECT MAX(lat_n) FROM station WHERE lat_n < 137.2345);
~~~

Here are the steps:
- Had to use 2 select statements.
- First, **I defined the condition required**: filter the lat_n lower than 137.2345 by using <code>WHERE lat_n = (SELECT MAX(lat_n) FROM station WHERE lat_n < 137.2345)</code>.
- Then, select the rounded long_w value limiting to 4 decimal places by using <code>ROUND(long_w, 4)</code>


Your Output (stdout)
```
117.2465
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-15/problem)
