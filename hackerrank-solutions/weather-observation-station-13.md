## Weather Observation Station 13

Query the sum of Northern Latitudes (LAT_N) from STATION having values greater than 38.7880 and less than 137.2345. 
Truncate your answer to 4 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT ROUND(SUM(LAT_N),4)
FROM STATION
WHERE LAT_N > 38.7880
    AND LAT_N < 137.2345;
~~~

Here are the steps:
- Used <code>ROUND(______,4)</code> to round the values limited to 4 decimal places.
- Used <code>WHERE LAT_N AND LAT_N < 137.2345> 38.7880</code> to considerate only lat_n values between 38.7880 and 137.2345.


Your Output (stdout)
```
36354.8135
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-13/problem)
