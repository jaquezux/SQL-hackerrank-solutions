## Weather Observation Station 11

Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT DISTINCT CITY
FROM STATION
WHERE CITY NOT REGEXP '^[aeiou].*[aeiou]$'
ORDER BY 1;
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>WHERE NOT</code> before <code>REGEXP '^[aeiou].*[aeiou]$'</code> to obtain cities that do not start OR do not end with vowels.

Your Output (stdout)
```
Addison 
Agency 
Alanson 
Albany 
Albion 
Algonac 
Allerton 
Alton 
Andover 
Anthony 
Arlington 
Arrowsmith 
Athens 
Auburn 
Baileyville 
Bainbridge 
Baker 
Baldwin 
Barrigada 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-11/problem)
