## Weather Observation Station 4

Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.
The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.

For example, if there are three records in the table with CITY values 'New York', 'New York', 'Bengalaru', there are 2 different city names: 'New York' and 'Bengalaru'. The query returns 1,  because total number of records - number of unique city names = 3 - 2 = 1.

## Solution:
~~~sql
SELECT COUNT(city) - COUNT(DISTINCT city)
FROM STATION;
~~~

Here are the steps:
- Used <code>COUNT</code> to find how many <i>city names</i> entries are in the table.
- Used <code>COUNT DISTINCT</code> to find how many cities are in the table, excluding duplicates.
- Used <code>-</code> to do the subtraction and find the difference.

Your Output (stdout)
```
13
```


[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-4/problem)
