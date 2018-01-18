                                                        #Movie Analysis
 
In this project, we have 6 problem statements to solve.

**Making a directory in HDFS**

hdfs dfs -mkdir '/moviedata/'

**Pushing data in HDFS**

hdfs dfs -put '/home/cloudera/Downloads/moviesdataset.txt' '/moviedata/' 

**Getting started with hive**

hive

**Creating a DB**

create database movie;

**Creating a table**

create table moviedata (id int, name string, year int, rating float, duration int)
    > row format delimited 
    > fields terminated by ','
    > ;

**Loading data into the table**

LOAD DATA INPATH '/moviedata/movies dataset for pig.txt'
    > INTO TABLE moviedata;

**Problem Statements**

1.**Find the number of movies released between 1950 and 1960.**

hive>SELECT count(*)  FROM moviedata
    > WHERE year BETWEEN 1950 AND 1960;

**OUTPUT** -  547

2.**Find the number of movies having rating more than 4.   **

hive> SELECT count(*)  FROM moviedata
    > WHERE rating > 4.0;

**OUTPUT** - 897

3.**Find the movies whose rating are between 3 and 4. **

hive> SELECT name  FROM moviedata
    > where rating > 3.0 and rating < 4.0;

**OUTPUT** - # Long List of Movies 

4.** Find the number of movies with duration more than 2 hours (7200 second).**

hive> SELECTcount (*) FROM moviedata 
    > WHERE duration > 7200;

**OUTPUT** - 641

5.**Find the list of years and number of movies released each year.**

hive> SELECT year, count (*) FROM moviedata
    > GROUP BY (year);

**OUTPUT** - Year     Number_of_movies
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx
	           xxxx	    xxxxxxxx


6.**Find the total number of movies in the dataset.**

hive> SELECT count (*) FROM moviedata;
 
 **OUTPUT** - 49590
