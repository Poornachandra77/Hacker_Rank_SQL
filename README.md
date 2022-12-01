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

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

SELECT City,State From Station;

8.  Weather Observation Station 3

Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer.
The STATION table is described as follows:


![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

SELECT DISTINCT CITY From Station WHERE MOD(ID,2) = 0 ;

9.  Weather Observation Station 4

Find the difference between the total number of CITY entries in the table and the number of distinct CITY entries in the table.
The STATION table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

SELECT COUNT(CITY) - COUNT(DISTINCT CITY) FROM STATION;

10.  Weather Observation Station 5

Query the two cities in STATION with the shortest and longest CITY names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.
The STATION table is described as follows:


![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) DESC, City ASC LIMIT 1;
SELECT CITY, LENGTH(CITY) FROM STATION ORDER BY LENGTH(CITY) ASC, City ASC LIMIT 1;

11. Weather Observation Station 6

Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. Your result cannot contain duplicates.
Input Format
The STATION table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

SELECT Distinct(CITY) FROM STATION WHERE CITY LIKE 'A%' OR CITY LIKE 'E%' OR CITY LIKE 'I%' OR CITY LIKE 'O%' OR CITY LIKE 'U%' ORDER BY CITY;

12. Weather Observation Station 7

Query the list of CITY names ending with vowels (a, e, i, o, u) from STATION. Your result cannot contain duplicates.
Input Format
The STATION table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

Select Distinct(City) From Station WHERE City like '%a' OR City like '%e' OR City like '%i' OR City like '%o' OR City like '%u' ORDER By CITY ASC;


13. Weather Observation Station 8

Query the list of CITY names from STATION which have vowels (i.e., a, e, i, o, and u) as both their first and last characters. Your result cannot contain duplicates.
Input Format
The STATION table is described as follows:

![alt text](https://github.com/Poornachandra77/Hacker_Rank_SQL/blob/main/hk2.jpeg?raw=true)

Solution:-

Select Distinct(City) from Station Where (City like 'A%' OR City like 'E%' OR City like 'I%' OR City like 'O%' OR City like 'U%') AND (City like '%a' OR City like '%e' OR City like '%i' OR City like '%o' OR City like '%u') ORDER BY City ASC;


