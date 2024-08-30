SELECT DISTINCT(CITY)
<br>
FROM STATION
<br>
WHERE 
<br>
CITY LIKE 'A%' 
<br>
OR CITY LIKE 'E%'
<br>
OR CITY LIKE 'I%'
<br>
OR CITY LIKE 'O%'
<br>
OR CITY LIKE 'U%';
<br>
<br>
Alternative:
<br>
SELECT DISTINCT CITY
<br>
FROM STATION
<br>
WHERE LEFT(CITY, 1) IN ('A', 'E', 'I', 'O', 'U');
