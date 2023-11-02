## Weather Observation Station 16

Query the smallest Northern Latitude (LAT_N) from STATION that is greater than 38.7780. Round your answer to 4 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT ROUND(MIN(lat_n), 4)
FROM station
WHERE lat_n > 38.7780;
~~~

Here are the steps:
- Used <code>ROUND(______,4)</code> to round the values limited to 4 decimal places.
- Used <code>WHERE lat_n > 38.7780</code> to get only values higher than 38.7780.

Your Output (stdout)
```
38.8526
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-16/problem)
