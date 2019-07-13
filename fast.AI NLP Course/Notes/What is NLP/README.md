# Fast AI 

This document contains my notes on the Fast AI NLP Course. :sparkles:

## A changing field

NLP has been changing quite a lot overtime. Initially, NLP relied on hard-coded rules about a language.  Later on it shifted towards using statistical and machine learning approaches. As of late, deep learning is now achieving state-of-the-art for many things.

## Summary of interesting blogs and articles

This section contains notes on some interesting blogs and articles

1.  **[How Vector Space Mathematics Reveals the Hidden Sexism in Language](https://www.technologyreview.com/s/602025/how-vector-space-mathematics-reveals-the-hidden-sexism-in-language/)**

    This article talks about the hidden sexism in Word2Vec dataset. 

    The Word2Vec algorithm was run on a corpus and the result was used to predict analgoies. The analogies turned out to be blatantly sexist. 

    A few researchers(Bolukbasi and co) tried to find a solution for this problem. They assumed the sexism present in the vector space as a kind of warping. And they though of removing this warping with the help of some methematical tools. 

    They cam up with a plan to apply an opposite warp in such a way that the overall vector space is still preserved. 

    The researchers looked for the warping  by searching the vector space for word pairs that produce a similar vector to “she: he.” They then fed this result to Amazon's Mechanical Turk to find out whether the result of sexist or not. 

    The truk ended up providing the researhers a list of pairs of analogies that were sexist. The researchers then came up with a way to transform the vector in a way that would remove the warping. They called this process ```hard-debiasing```. 

    The end result is a vector space in which the gender bias is significantly reduced.

    *Applications* - 

    > Any bias contained in word embeddings like those from Word2vec is automatically passed on in any application that exploits it. One example is the work using embeddings to improve Web search results. If the phrase “computer programmer” is more closely associated with men than women, then a search for the term “computer programmer CVs” might rank men more highly than women. “Word embeddings not only reflect stereotypes but can also amplify them,” say Bolukbasi and co.   

    More information can be found in this [paper](https://arxiv.org/pdf/1607.06520.pdf).

1.  **[Lipstick on a Pig:Debiasing Methods Cover up Systematic Gender Biasesin Word Embeddings But do not Remove Them](/https://arxiv.org/pdf/1903.03862.pdf)**

    This is a quite an interesting paper which talks about how the de-biasing methodoligies do not completely remove the gender bias from the word embeddings.  

    This paper mentions two de-biasing methods which were develeoped by - 

    1.  Bolukbasi et al.
    1.  Zhao et al.

    The paper also mentions experiments which show how gender bias still prebails in the word embedding matrix even after debiasing it.

    > This  clustering  of  gendered  wordsindicates that while we cannot directly “observe”the  bias  (i.e.    the  word  “nurse”  will  no  longerbe  closer  to  explicitly  marked  feminine  words)the  bias  is  still  manifested  by  the  word  beingclose   tosocially-markedfeminine   words,   forexample  “nurse”  being  close  to  “receptionist”,“caregiver”  and  “teacher”.  

    > The crux of the issue is that the gender-directionprovides a way tomeasurethe gender-associationof a word,  butdoes not determineit.   Debiasingmethods which directly target the gender-directionare for the most part merely hiding the gender biasand not removing it. The popular definitions usedfor quantifying and removing bias are insufficient,and other aspects of the bias should be taken intoconsideration as well

1.  **[How Will We Prevent AI-Based Forgery?](https://hbr.org/2019/03/how-will-we-prevent-ai-based-forgery)**   

    This is a very interesting article that talks about how deep learning can cause serious issues. With the advancement in deep learning algorithms, it has become quite easy to produce fakes such as **deep fakes**. 

    [This](https://grail.cs.washington.edu/projects/AudioToObama/siggraph17_obama.pdf) is also an interesting read. This paper is about creating Lip synced video from an audio file. The technology mentioned in this paper can be used to drastically improve video calls. 

    [Here](https://www.vice.com/en_us/article/bjye8a/reddit-fake-porn-app-daisy-ridley) is another creepy article that shows what happens if deepfakes fall into the wrong hands.

1.  **[Introduction to ME-ULMFiT](https://www.novetta.com/2019/03/introducing_me_ulmfit/)**

    This is yet another intresting article that talks about an enhanced meta-data enhanced ULMFiT algorithm. 
