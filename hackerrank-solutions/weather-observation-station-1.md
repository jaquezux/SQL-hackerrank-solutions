## Weather Observation Station 1

Query a list of CITY and STATE from the STATION table.
The STATION table is described as follows:

<img src="https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg">

where LAT_N is the northern latitude and LONG_W is the western longitude.

## Solution:
~~~sql
SELECT city, state
FROM station;
~~~

Your Output (stdout)
```
Acme LA 
Addison MI 
Agency MO 
Aguanga CA 
Alanson MI 
Alba MI 
Albany CA 
Albion IN 
Algonac MI 
Aliso Viejo CA 
Allerton IA 
Alpine AR 
Alton MO 
Amazonia MO 
Amo IN 
Andersonville GA 
Andover CT 
Anthony KS 
Archie MO 
```

Here are the steps:
- Used <code>city</code> and <code>state</code> to select city and state fields from STATION table.

[Check the problem here.](https://www.hackerrank.com/challenges/weather-observation-station-1/problem)
