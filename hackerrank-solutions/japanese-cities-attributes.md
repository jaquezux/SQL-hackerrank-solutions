## Japanese Cities' Attributes
Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.

The CITY table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg">

## Solution:
~~~sql
SELECT *
FROM city
WHERE countrycode = 'JPN';
~~~

Your Output (stdout)
```
1613 Neyagawa JPN Osaka 257315
1630 Ageo JPN Saitama 209442
1661 Sayama JPN Saitama 162472
1681 Omuta JPN Fukuoka 142889
1739 Tokuyama JPN Yamaguchi 107078
```

Here are the steps:
- Used the <code>*</code> to select all fields from City table.
- Used <code>WHERE</code> statement to filter only for "JPN" CountryCode.

[Check the problem here.](https://www.hackerrank.com/challenges/japanese-cities-attributes/problem)
