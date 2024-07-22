# HR-Solution-Weather-Observation-Station-13
Solutions for MySQL and SQL Server

## PROBLEM
Query the sum of Northern Latitudes (LAT_N) from STATION having values greater than 38.7880 and less than 137.2345. Truncate your answer to decimal places.

## SQL SERVER:
SELECT CAST(ROUND(SUM(LAT_N),4) AS DECIMAL(16, 4))
FROM STATION 
WHERE LAT_N BETWEEN 38.7880 AND 137.2345;

OR

SELECT CAST(ROUND(SUM(LAT_N),4) AS NUMERIC(36, 4))
FROM STATION 
WHERE LAT_N BETWEEN 38.7880 AND 137.2345;

## MySQL:
SELECT ROUND(SUM(LAT_N), 4)
FROM STATION
WHERE LAT_N BETWEEN 38.7880 AND 137.2345;


