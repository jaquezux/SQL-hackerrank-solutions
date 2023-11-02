## Weather Observation Station 14

Query the greatest value of the Northern Latitudes (LAT_N) from STATION that is less than 137.2345. Truncate your answer to 4 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT MAX(ROUND(LAT_N, 4))
FROM station
WHERE lat_n < 137.2345;
~~~

Here are the steps:
- Used <code>ROUND(______,4)</code> to round the values limited to 4 decimal places.
- Used <code>MAX()</code> to get the greatest value of the Northern Latitudes (LAT_N).
- But the problem gave the condition to get a value **lower than 137.2345**, because of this, I used <code>WHERE lat_n < 137.2345</code> to filter.


Your Output (stdout)
```
137.0193
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-14/problem)
