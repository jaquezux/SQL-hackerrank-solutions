## Revising the Select Query II
Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.

The CITY table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg">

## Solution:
~~~sql
SELECT name
FROM city
WHERE countrycode = 'USA'
    AND population > 120000;
~~~

Here are the steps:
- Used the <code>name</code> to select only name field.
- Used <code>WHERE</code> statement to filter only for "USA" CountryCode.
- Used <code>AND</code> in <code>WHERE</code> statement to filter only population above 120000.

[Check the problem here.](https://www.hackerrank.com/challenges/revising-the-select-query-2/problem)
