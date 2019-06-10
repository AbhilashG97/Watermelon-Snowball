# Singular Value Decomposition 

This section contains notes on ```Singular Value Decomposition```, commonly abbreviated as ```SVD```. 

## Prerequisites

Before, we dive into SVD, let's have a look at a few things first.

### Points and Space

:star: Space represented by more than three dimensions is called **hyperspace**.

:warning:  Also, the term n-space used to talk about spaces of different dimensionality (e.g. 1-space, 2-space, ..., n-space).

### Vectors Revisited 

> The inner product of two vectors (also called the dot product or scalar product) defines multiplication of vectors. It is found by multiplying each component in v~1 by the component in v~2 in the same position and adding them all together to yield a scalar value.

:warning: If the ```dot product``` of two vectors equals zero, then the two vectors are said to be orthogonal to each other.

#### Normal Vectors 

A ```normal vector``` or a unit vector is a vector of unit lenght. It calculated by dividing a vector by its magnitude. 

### Orthonormal Vectors

Vectors of **unit length** that are **orthogonal** to each other are said to be ```orthonormal```.

### Gram-Schmidt Orthonormalization Process

This is a method for converting a set of vectors into a set of orthonormal vectors.

Given an orthonormal set of vectors ```u```<sub>```1```</sub>, ```u```<sub>```1```</sub>, ...., ```u```<sub>```k-1```</sub>, then ```w```<sub>```k```</sub>

<p align="center"><img src ="https://github.com/AbhilashG97/Watermelon-Snowball/blob/master/Deep%20NLP%20-%20Stanford%20University/Day%201/images/gram-schmidt.png"/></p>

### Orthogonal Matrices

A matrix ```A``` is said to be orthogonal, if the following is true -

<p align="center"><img src ="https://github.com/AbhilashG97/Watermelon-Snowball/blob/master/Deep%20NLP%20-%20Stanford%20University/Day%201/images/orthogonal-matrix.png"/></p>

### Determinant 

> It is a function of a square matrix that reduces it to a single number.

### Eigenvalue and Eigenvectors 

An eigenvector is a nonzero vector that satisfies the equation below - 

<p align="center"><img src ="https://github.com/AbhilashG97/Watermelon-Snowball/blob/master/Deep%20NLP%20-%20Stanford%20University/Day%201/images/eigen.png"/></p>

where A is a square matrix, ```λ``` is a scalar, and ```v``` is the eigenvector. ```λ``` is called an eigenvalue. Eigenvalues and eigenvectors are also known as, respectively, characteristic roots and characteristic vectors, or latent roots and latent vectors.

### Singular Value Decomposition (SVD)

It is primarily used for dimensionality reduction. It can be expressed by the following equation - 

<p align="center"><img src ="https://github.com/AbhilashG97/Watermelon-Snowball/blob/master/Deep%20NLP%20-%20Stanford%20University/Day%201/images/svd.png"/></p>

SVD is based on a theorem from linear algebra which says that a rectangular matrix A can be broken down into the product of three matrices - an orthogonal matrix ```U```, a diagonal matrix ```S```, and the transpose of an orthogonal matrix ```V```.

:boom: The columns of ```U``` are orthonormal eigenvectors of AA<sup>T</sup>, the columns of ```V``` are orthonormal eigenvectors of A<sup>T</sup>A, and ```S``` is a diagonal matrix containing the square roots of eigenvalues from ```U``` or ```V``` in descending order.
