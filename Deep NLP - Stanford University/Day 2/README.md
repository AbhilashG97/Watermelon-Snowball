# DAY TWO - WORD VECTOR REPRESENTATIONS: word2vec

## How do we represent the meaning of a word?

Word Vectors are primarily used to represent the meaning of a word.

## How do we have usable meaning in a computer? 

A common taxonomy like ```WordNet``` that has hypernymes (is-a) relationships and sysnonym sets.

### Hypernym vs Hyponym

> In simpler terms, a hyponym is in a type-of relationship with its hypernym. For example, pigeon, crow, eagle and seagull are all hyponyms of bird (their hypernym); which, in turn, is a hyponym of animal.

[!hypernym-vs-hyponym](#image)

## Problems with descrete representation 

There are a few problems with ```WordNet``` which are mentioned below - 

1.  Great as a resource but missing nuances.

    For instance, synonymes for good can be adept, expert, good, practiced, proficient, skillful etc, but all of these words denote a varying level of meaning. 

    For instance, when someone says that they are *good at something* and when they say they are *expert at something*; both of these sentences have a subtle difference albeit the words good and expert are synonymes.

1.  Missig new words. 

    WordNet is not able to keep track of all the new words being introduced to a language. 

1.  Requires human labour to create and adapt. 

### One-Hot representation

It is a ```localist``` represenatation. It consists of a vector space of ```zeros``` and ```ones```. The vector space is marked with ```one```, if the word matches a word present in word vector.  

One-Hot encoding is used to perform ```binarization```. It converts a ```feature set``` to a ```binary feature set```.

:boom: It is a symbolic representation. 

#### Why are One-Hot representations bad?

```One-Hot```representation cannot be used to find the similarity between words. It doesn't give us the measure as to how similar a word is to another word. 

:warning: There is no natural notion of similarity in a set of one-hot vectors.

:exclamation: Let us consider an example where we have two sentences which contains the word ```hotel``` and ```motel```. If we represent the one-hot encoding of the two words by ```x``` and ```y```, and then evaulate ```x transpose . y``` the result will turn out to be zero.

## Distributional similarity based representations

Here, a word is given a weight depending upon the neighbouring words (also known as context words).

> Effectively, Word2Vec/Doc2Vec is based on distributional hypothesis where the context for each word is its nearby words. Similarly, LSA takes the entire document as the context. Both techniques solve the word embedding problem - embed words into a continuous vector space while keeping semantically related words close together.

> On the other hand, LDA isn't made to solve the same problem. They deal with a different problem called topic modeling, which is finding latent topics in a set of documents.

:warning: Please read this StackOverflow post on the difference between ```distributed representation``` and ```distributional representation```. 

## Basic idea of learning neural network word embeddings

