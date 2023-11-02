Write a query that prints a list of employee names (i.e.: the name attribute) for employees in Employee having a salary greater than  per month who have been employees for less than  months. Sort your result by ascending employee_id.

Input Format

The Employee table containing employee data for a company is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/19629/1458557872-4396838885-ScreenShot2016-03-21at4.27.13PM.png" width="150">

where employee_id is an employee's ID number, name is their name, months is the total number of months they've been working for the company, and salary is the their monthly salary.


Sample Input:

<img src="https://s3.amazonaws.com/hr-challenge-images/19630/1458558612-af3da3ceb7-ScreenShot2016-03-21at4.32.59PM.png" width="200">

<br/>

**Explanation**


- Angela has been an employee for 1 month and earns $3443 per month.
- Michael has been an employee for 6 months and earns per $2017 month.
- Todd has been an employee for 5 months and earns $3396 per month.
- Joe has been an employee for 9 months and earns $3573 per month.

We order our output by ascending employee_id.

## Solution:
~~~sql
SELECT name
FROM employee
WHERE salary > 2000
    AND months < 10
ORDER BY employee_id ASC;
~~~

Here are the steps:
- Used <code>WHERE salary > 2000</code> to filter only employees that earn more than $2000.
- Used <code>AND months < 10</code> to filter only employees with more than 10 months in the company.
- Used <code>ORDER BY employee_id ASC</code> to sort by ID ascending.

Your Output (stdout)
```
Rose 
Patrick 
Lisa 
Amy 
Pamela 
Jennifer 
Julia 
Kevin 
Paul 
Donna 
Michelle 
Christina 
Brandon 
Joseph 
Jesse 
Paula 
Louise 
Evelyn 
Emily 
```

[Check the problem here.](https://www.hackerrank.com/challenges/salary-of-employees/problem)
