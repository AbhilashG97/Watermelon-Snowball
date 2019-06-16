# DAY TWO - WORD VECTOR REPRESENTATIONS: word2vec

This document contains my notes on whatever that was taught on Day 2 of the Deep NLP Course.

## Sparse Matrix and Sparcity 

Please have a look [here](https://machinelearningmastery.com/sparse-matrices-for-machine-learning/) for more information.

A **sparse matrix** is a matrix that consists of mostly zero values.

A **dense matrix** on the other hand is a one that consists of mostly non-zero values. 

The **sparsity** of a matrix can be quantified with a score, which is the number of zero values in the matrix divided by the total number of elements in the matrix.

              number of zero valued elements 
 sparcity  =  ------------------------------ 
                 total number of elements    

#### Problems with sparcity

The following problems occur due to sparse matrices - 

1. **Space Complexity**
   
   Very large matrices require a lot of memory and most of large matrices in ML are sparse. This is a waste of memory resources as zero values do not contain any information.

2. **Time Complexity**

   If the matrix contains mostly zero-values, i.e. no data, then performing operations across this matrix may take a long time where the bulk of the computation performed will involve adding or multiplying zero values together.

#### How to deal with sparse matrices

```Scipy``` and ```Numpy``` provide various functions which can be used to convert sparse matrices into dense matrices.


## Skip-Gram model with negative sampling

**Main idea:** Train binary logistic regressions for a true pair (center word and word in its context window) versus several noise pairs (the center word paired with a random word)

You can find more information by reading [this paper](http://papers.nips.cc/paper/5021-distributed-representations-of-words-and-phrases-and-their-compositionality.pdf).

