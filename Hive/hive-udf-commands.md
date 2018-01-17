**We need to create a *temporary function* in hive to use the UDF**:

create temporary function "user-defined function name" as "Java code class name";

**To execute**:

select id,"user-defined function name"(column name) from tablename;
