# What is it?

*Apache Spark* is a *cluster computing platform* widely used in [[Data Engineering]], designed to be **fast** and **general-purpose**. It extends other [[Distributed Computing]] frameworks like [[Hadoop]], and the [[MapReduce]] model to **efficiently handle** all needed workload. This is done mainly through the [[Resilient Distributed Datasets]] concept, which is *Spark*'s **main programming abstraction**.

![[spar.png]]

The *Spark* engine is **designed to be flexible enough** to cover wide ranges of workloads, including *batch processing*, *iterative [[Algorithms|algorithms]]*, *queries* and *stream processing*. *Spark* also offers [[API|APIs]] in [[Python]], [[Java]], [[Scala]], and *SQL*.
___
# Spark components

A *Spark* cluster could integrate many **different components** which have their own use-cases, like the [[Hadoop]] ecosystem. However, the **inner working** of *Spark* could be **generalized to five components**:

![[spark components.png]]

- ##### Spark Core
	Contains **basic functionality**, like **task scheduling**, **memory management**, **fault recovery**, and **storage interaction**. *Spark Core* houses the [[API]] which defines [[Resilient Distributed Datasets]].

- ##### Spark SQL
	*Spark SQL* is a interface which allows querying structured data, using [[SQL]]