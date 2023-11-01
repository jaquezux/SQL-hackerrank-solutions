## Weather Observation Station 3

Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.

## Solution:
~~~sql
SELECT DISTINCT CITY
FROM STATION
WHERE ID % 2=0;
~~~

Here are the steps:
- Used <code>DISTINCT</code> to select the cities in STATION table excluding duplicates.
- Used <code>%</code> to filter only even IDs.

Your Output (stdout)
```
Aguanga 
Alba 
Albany 
Amo 
Andersonville 
Archie 
Athens 
Atlantic Mine 
Bainbridge 
Baker 
Bass Harbor 
Bayville 
Beaufort 
Bellevue 
Benedict 
Bennington 
Bentonville 
Biggsville 
Bison 
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-3/problem)
