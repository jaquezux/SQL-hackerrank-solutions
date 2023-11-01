## Japanese Cities' Names

Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.
The CITY table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg">

## Solution:
~~~sql
SELECT name
FROM city
WHERE countrycode = 'JPN';
~~~

Your Output (stdout)
```
Neyagawa 
Ageo 
Sayama 
Omuta 
Tokuyama 
```

Here are the steps:
- Used the <code>name</code> attribute to select only NAME field from CITY table.
- Used <code>WHERE</code> statement to filter only for "JPN" CountryCode.

[Check the problem here.](https://www.hackerrank.com/challenges/japanese-cities-name/problem)
