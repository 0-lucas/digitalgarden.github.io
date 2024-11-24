# What is it?

In the book [[Nathan Marz, James Warren Big Data Principles and best practices of scalable realtime data systems.pdf|Big Data - Principles and Best Practices]], *Nathan Marz* and *James Warren* proposed a new [[Architecture Patterns|architecture pattern]] for [[Big Data]] systems which **accomplish both** *batch processing* and *stream processing*, with **one or more** *pipelines*.

This is the *lambda architecture*. It proposes that a [[Big Data]] system should be **build upon three layers**, each responsible for a **different facet of the system**.

![[lambda.png]]
___
# The layers of lambda