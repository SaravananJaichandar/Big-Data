**Sqoop Help**:

sqoop help

**To list tables**:

sqoop list-tables --connect jdbc:mysql://localhost/loudacre --username root --password cloudera  (Incase of cloudera Virtual machine)

**To create a directory with same name as that of table name in hdfs**:

sqoop import --connect jdbc:mysql://localhost/databasename --username root --password cloudera --table calllog --fields-terminated-by ':' --warehouse-dir '/databasename'

**For increamental Approach**:

sqoop import --connect jdbc:mysql://localhost/databasename --username root --password cloudera --incremental append --null-non-string '\\N' --table accounts --target-dir /databasename/accounts --check-column acct_num --last-value 97349

**To Print the results without logging into Mysql**:

sqoop eval --query "SELECT * FROM webpage LIMIT 10" --connect jdbc:mysql://localhost/databasename --username root --password cloudera
