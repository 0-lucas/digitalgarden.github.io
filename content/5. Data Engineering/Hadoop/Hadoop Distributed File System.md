# What is it?

The *HDFS*, which stands for *[[Apache Hadoop|Hadoop]] Distributed File System*, is a data storage technique designed to **handle massive amounts of data**. It handles the data by **partitioning it into smaller pieces**.

![[Pasted image 20241110132533.png]]
___
# The write-once, read-many approach

*HDFS* is built around the idea that the file will be **written only once**, but will be **read multiple times**. This way, it focuses on **fastest retrieval time**, while **not allowing to edit existing data**.

