## Weather Observation Station 17

Query the Western Longitude (LONG_W)where the smallest Northern Latitude (LAT_N) in STATION is greater than 38.7780. Round your answer to 4 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT ROUND(long_w,4)
FROM station 
WHERE lat_n IN (
    SELECT MIN(lat_n)
    FROM station
    WHERE lat_n > 38.7780
    );
~~~

Here are the steps:
- I had to use 2 select statements.
- First, I defined the condition required: **get the minimum lat_n higher than 38.770** by using <code>MIN(lat_n)</code> and <code>WHERE lat_n > 38.7780</code>.
- Then, I selected the long_w value using <code>ROUND(______,4)</code> to round the values limited to 4 decimal places.

Your Output (stdout)
```
70.1378
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-17/problem)
