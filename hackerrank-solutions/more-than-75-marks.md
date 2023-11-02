Query the Name of any student in STUDENTS who scored higher than 75 Marks. Order your output by the last three characters of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending ID.

Input Format

The STUDENTS table is described as follows: 

<img src="https://s3.amazonaws.com/hr-challenge-images/12896/1443815243-94b941f556-1.png" width="200">

The Name column only contains uppercase (A-Z) and lowercase (a-z) letters.

Sample Input:

<img src="https://s3.amazonaws.com/hr-challenge-images/12896/1443815209-cf4b260993-2.png" width="200">

<br/>

**Explanation**

Only Ashley, Julia, and Belvet have Marks > . If you look at the last three characters of each of their names, there are no duplicates and 'ley' < 'lia' < 'vet'.

## Solution:
~~~sql
SELECT Name
FROM STUDENTS
WHERE Marks > 75
ORDER BY RIGHT(Name, 3), ID ASC;
~~~

Here are the steps:
- Used <code>WHERE > 75</code> to filter only students with more than 75 marks.
- Used <code>RIGHT (Name, 3)</code> to order considering the 3 ending caracters from each Name.
- Used <code>ID ASC</code> as a secondary order statement, so if there are students ending with the same caracters, the ID would be considered to sort.

Your Output (stdout)
```
Stuart 
Kristeen 
Christene 
Amina 
Aamina 
Priya 
Heraldo 
Scarlet 
Julia 
Salma 
Britney 
Priyanka 
Samantha 
Vivek 
Belvet 
Devil 
Evil
```

[Check the problem here.](https://www.hackerrank.com/challenges/more-than-75-marks/problem)
