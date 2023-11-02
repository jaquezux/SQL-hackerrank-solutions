## Weather Observation Station 2

Query the following two values from the STATION table:

1. The sum of all values in LAT_N rounded to a scale of 2 decimal places.
2. The sum of all values in LONG_W rounded to a scale of 2 decimal places.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg" width="150">

where LAT_N is the northern latitude and LONG_W is the western longitude.


Output Format

Your results must be in the form:
```
lat lon
```

where lat is the sum of all values in LAT_N and lon is the sum of all values in LONG_W. Both results must be rounded to a scale of 2 decimal places.


## Solution:
~~~sql
SELECT ROUND(SUM(LAT_N),2), ROUND(SUM(LONG_W),2)
FROM STATION;
~~~

Here are the steps:
- Used <code>ROUND</code> and <code>SUM</code>.
- <code>ROUND(______,2)</code> to round the values limited to 2 decimal places.
- <code>SUM(LAT_N)</code> to sum all values from LAT_N field.
- <code>SUM(LONG_W)</code> to sum all values from LONG_W field.


Your Output (stdout)
```
42850.04 47381.48
```



[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-2/problem)
