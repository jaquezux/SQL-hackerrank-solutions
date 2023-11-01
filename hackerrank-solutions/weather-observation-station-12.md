## Weather Observation Station 12

Query the list of CITY names from STATION that do not start with vowels and do not end with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT REGEXP '^[aeiou]'
    AND CITY NOT REGEXP '[aeiou]$'
ORDER BY 1;
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>WHERE NOT</code> before <code>REGEXP '^[aeiou]'</code> to obtain only cities that do not start with vowels.
- Used <code>AND NOT</code> before <code>REGEXP '[aeiou]$'</code> to obtain only cities that do not end with vowels.

Your Output (stdout)
```
Baker 
Baldwin 
Bass Harbor 
Beaufort 
Beaver Island 
Benedict 
Bennington 
Berryton 
Beverly 
Bison 
Blue River 
Bowdon 
Bowdon Junction 
Bridgeport 
Bridgton 
Brighton 
Brilliant 
Bristol 
Brownstown 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-12/problem)
