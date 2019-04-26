# DAY ONE -  Natural Language Processing with Deep Learning

## Intorduction 

**What is Natural Language Processing (NLP)?**

Natural Language Processing is a field at the intersection of 

1. computer science
1. artificial intelligence
1. and linguistics. 

The **goal** is to process natural language in order to perform tasks that are useful. 

### NLP Levels 

The whole NLP process can be divided into variuos levels which is shown below - 

![nlp-levels](#nlp-levels)

### What's special about human language?

A human language is a system specifically constructed to convey the speaker/writer's meaning. 

Unlike, other forms of data, human language is very well constructed and usually contains some meaning. 

:warning: A human language is a **descrete/symbolic/categorical** signalling system.  

:boom: Humans communicate using sound, gesture and images.

### What's Deep Learning?

Machine learning in general can be summed up somewhat like this in general - 

```ML in practice = Describing your data with features a computer can understand + Learning Algorithm```

```Deep Learning``` algorithms attempt to learn (multiple levels of) representation and an output

```Representation learning``` attempts to automatically learn good features or representations from raw inputs like sound, characters or words.

Deep Learning does not necessarily always have to use Neural Networks, it can also use other probabilistic models.

### Reasons for exploring Deep Learning

Below mentioned are some reasons why Deep Learning needs to be explored - 

1. Manually designed features are often over-specified, incomplete and take a long time to design and validate.

1. **Learned Features** are easy to adapt, fast to learn. 

1. Deep Learning can learn ```unsupervised```(from raw text) and ```supervised```(with specific labels like positive/negative)

1. Improved performance (Speech recognition and Computer Vision). 

There are many other reasons as well.

### Deep NLP 

Combine ideas and goals of NLP with using representation learning and deep learning methods to solve them.

**```Morpheme```** - a meaningful morphological unit of a language that cannot be further divided.

```Deep Learning method -```

1. Every word and every phrase and every logical expression is a vector.

1. A neural network combines two vectors into one vector.

:warning: More on this later.

### Dialog Agents / Response Generation 

An application of the powerful, general technique of ```Natural Language Model```, which are an instance of ```Recurrent Neural Network```.

Google's Inbox replies uses RNN to read the mail, it then suggests replies depending on the context of the mail.

### Neural Machine Translation 

Source sentence is mapped to a vector, then output senetence is generated.

### Important Resources

1. https://nlp.stanford.edu/pubs/snli_paper.pdf
1. https://nlp.stanford.edu/~lmthang/data/papers/conll13_morpho.pdf
1. https://arxiv.org/abs/1604.00788
1. https://arxiv.org/abs/1409.0473
1. https://arxiv.org/abs/1409.3215
