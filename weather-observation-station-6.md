## Weather Observation Station 6

Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT DISTINCT CITY 
FROM STATION 
WHERE CITY REGEXP '^[aeiou]'
ORDER BY city;
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>REGEXP '^[aeiou]'</code> to filter city names starting with vowels.
- Ordered by city, ASC by default.

Your Output (stdout)
```
Acme 
Addison 
Agency 
Aguanga 
Alanson 
Alba 
Albany 
Albion 
Algonac 
Aliso Viejo 
Allerton 
Alpine 
Alton 
Amazonia 
Amo 
Andersonville 
Andover 
Anthony 
Archie 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-6/problem)
