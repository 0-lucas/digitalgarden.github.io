# The shared-nothing architecture

In [[Data Engineering]], an [[Apache Hadoop]] *cluster* is a **group of computers**, which can be called *nodes*, that act as a **single system working on the same task**. Each *node* is its own machine, with isolated memory and disk which is **not shared between other nodes**.

This is called the [[Shared Nothing Architecture]], which enables better [[Scaling|scalability]], and makes the *cluster* **fault-tolerant to any failing node**, which can quickly recover, **not impacting other nodes**.

![[hadoop shared nothing.png]]
___
# The cluster architecture

While *nodes* are independent bet