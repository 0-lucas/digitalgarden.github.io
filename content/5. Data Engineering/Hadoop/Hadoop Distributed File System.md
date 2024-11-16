# What is it?

The *HDFS*, which stands for *[[Apache Hadoop|Hadoop]] Distributed File System*, is a data storage technique designed to **handle massive amounts of data**, be **fault tolerable**, while still being able to **[[Scaling|scale]] with standard machines**.

![[hadoop file.png]]
___
# The write-once, read-many approach

*HDFS* is built around the idea that the file will be **written only once**, but will be **read multiple times**. This way, it focuses on **fastest retrieval time**, while **not allowing to edit existing data**. 
This happens because the *writer module* has a lock to ensure **data coherency**, which would be **prejudiced** if a large file was to be **read and written at the same time**.

>[!tip] How to *kinda* update records?
>  While is not possible to update a existing record in-place, one could just **delete the old record** and **insert an updated copy** at the **same place** the old record was.

___
# The architecture of HDFS

*HDFS* has two main components: *Name Nodes* and *Data Nodes*