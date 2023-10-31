## Revising the Select Query I
Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.

The CITY table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg">

## Solution:
~~~sql
SELECT *
FROM city
WHERE countrycode = 'USA'
    AND population >= 100000;
~~~

Here are the steps:
- Used the <code>*</code> to select all columns.
- Used <code>WHERE</code> statement to filter only for "USA" CountryCode.
- Used <code>AND</code> in <code>WHERE</code> statement to filter only population above 100000.

[Check the problem here.](https://www.hackerrank.com/challenges/revising-the-select-query/problem)
