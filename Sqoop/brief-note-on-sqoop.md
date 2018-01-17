#Sqoop

Sqoop is developed for Sql developers, to transfer mysql data to hdfs and vice-versa, so that the sql code they write is converted into map-reduce and applied to data for data analysis.

**Working of Sqoop** :

  1.Sqoop will not work if the table does not have a *Primary key*.
  2.The Primary key should be *Numeric*.
  3.In Sqoop, there is only mapper code and no reducer code.
  4.By default, Sqoop will create 4 mappers.
  5.It selects the MAX,MIN from the primary key in the table and sets them in 4 mappers.
  
**Incremental Approach in Sqoop**:

Hadoop follows **WORM** principle - Write Once, Read Many. 
So Row-level addition or deletion is not allowed in hadoop environment, So when the file we transfered to hdfs from mysql gets updated, we can use this *Incremental approach*, so that a new file is created for the updated data.
