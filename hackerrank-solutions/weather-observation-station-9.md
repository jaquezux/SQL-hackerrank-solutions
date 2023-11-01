## Weather Observation Station 9

Query the list of CITY names from STATION that do not start with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT REGEXP '^[aeiou]'
ORDER BY CITY;
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>WHERE NOT</code> before <code>REGEXP '^[aeiou]'</code> to obtain cities that do not start with vowels.

Your Output (stdout)
```
Baileyville 
Bainbridge 
Baker 
Baldwin 
Barrigada 
Bass Harbor 
Baton Rouge 
Bayville 
Beaufort 
Beaver Island 
Bellevue 
Benedict 
Bennington 
Bentonville 
Berryton 
Bertha 
Beverly 
Biggsville 
Bison 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-9/problem)
