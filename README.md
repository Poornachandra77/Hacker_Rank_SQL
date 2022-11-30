# Hacker_Rank_SQL

1.  Revising The Select Query 1

Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT * FROM CITY
WHERE POPULATION > 100000 AND COUNTRYCODE = 'USA';


