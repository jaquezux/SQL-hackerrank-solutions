Write a query that prints a list of employee names (i.e.: the name attribute) from the Employee table in alphabetical order.

Input Format

The Employee table containing employee data for a company is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/19629/1458557872-4396838885-ScreenShot2016-03-21at4.27.13PM.png" width="150">

where employee_id is an employee's ID number, name is their name, months is the total number of months they've been working for the company, and salary is their monthly salary.

Sample Input:

<img src="https://s3.amazonaws.com/hr-challenge-images/19629/1458558202-9a8721e44b-ScreenShot2016-03-21at4.32.59PM.png" width="200">


## Solution:
~~~sql
SELECT name
FROM employee
ORDER BY name ASC;
~~~

Here are the steps:
- Select <code>name</code> field.
- Sorted by <code>name ASC</code> to get alphabetical order.

Your Output (stdout)
```
Alan 
Amy 
Andrew 
Andrew 
Angela 
Ann 
Anna 
Anthony 
Antonio 
Benjamin 
Bonnie 
Brandon 
Brandon 
Brian 
Carol 
Charles 
Christina 
Christina 
Christine 
```

[Check the problem here.](https://www.hackerrank.com/challenges/name-of-employees/problem)
