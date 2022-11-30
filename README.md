# Hacker_Rank_SQL

1.  Revising The Select Query I

Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT * FROM CITY WHERE POPULATION > 100000 AND COUNTRYCODE = 'USA';

2.  Revising the Select Query II

Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT NAME FROM CITY WHERE Population >120000 AND CountryCode = 'USA';

3.   Select All

Query all columns (attributes) for every row in the CITY table.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT * FROM CITY;

4.  Select By ID

Query all columns for a city in CITY with the ID 1661.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT * From CITY WHERE ID = 1661;

5.  Japanese Cities' Attributes

Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT * FROM CITY WHERE COUNTRYCODE = 'JPN';

6.  Japanese Cities' Names

Query the names of all the Japanese cities in the CITY table. The COUNTRYCODE for Japan is JPN.
The CITY table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT Name FROM city WHERE Countrycode = 'JPN';

7.  Weather Observation Station 1

Query a list of CITY and STATE from the STATION table.
The STATION table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk1.jpeg?raw=true)

Solution:-

SELECT City,State From Station;
