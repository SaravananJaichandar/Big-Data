**Hive**

Hive was developed by Facebook to facilitate the sql developers to convert their mysql queries into mapreduce and perform the desired quering operations.
Hive Queries are called as *HQL Query*.

**Schema-On-Read**:

Validation is performed while reading rather than writing because it is less-expensive.

**Working of Hive**:

  1.Parse HQL Queries - verify syntax
  2.Make Optimizations - make optimized map reduce programs
  3.Plan Execution - Plan which line in the query to execute first
  4.Submit jobs to cluster
  5.Monitor Progress
  
**Advanced Concepts in Hive**

1.**Partitioning**:

Partitioning a file into number of sub-files to increase the performance.

2.**Sub-Partitioning**:

Partitioning inside another partition.

3.**Bucketing**:

Bucketing uses random hash algorithm. We can manually restrict the number of sub-partitions we want.
