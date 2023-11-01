## Weather Observation Station 8

Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.

Input Format

The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.


## Solution:
~~~sql
SELECT DISTINCT CITY
FROM STATION
WHERE CITY REGEXP '^[aeiou].*[aeiou]$';
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>REGEXP '^[aeiou].*[aeiou]$'</code> to obtain only cities starting and ending with vowels.

Your Output (stdout)
```
Acme 
Aguanga 
Alba 
Aliso Viejo 
Alpine 
Amazonia 
Amo 
Andersonville 
Archie 
Arispe 
Arkadelphia 
Atlantic Mine 
East China 
East Irvine 
Eastlake 
Eleele 
Elm Grove 
Eriline 
Ermine 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-8/problem)
