# What is it?

The *Term-frequency representation*, also referred as *TF*, for short, is a way of **representing sentences in [[Vectors]]**, **counting each word** and adding to the its index in the vector. It's different from the [[One-Hot Vectorization]], where a index can go up to an infinite sum of its present words.

It's widely used in [[Natural Language Processing]] and [[Large Language Models]] for [[Deep Learning]] purposes.
___
# How does it work?

For a given sentence `time flies like fruit flies`, one can assume an *one-dimensional vector* with length equal to the **sum of distinct words** in the sentence. 
For our example, this would yield in a vector with length of $4$. We could also represent our vector like this:

$$
V_{words} = [time, flies, like, fruit]
$$

Now, we count the presence of each word and assign its **sum to its corresponding index**. Because the word ``
