# Summary of Neural networks generalize because of this one weird trick
by Jesse Hoogland
[link](https://www.lesswrong.com/posts/fovfuFdpuEwQzJu2w/neural-networks-generalize-because-of-this-one-weird-trick)

## TLDR

## Post structure
Intro (basic problems and ideas)
Back to the Bayes-ics
Statistical learning theory is built on a lie
Learning is physics with likelihoods
Why "singular"?
Phase transitions are singularity manipulations
Neural networks are freaks of symmetries
Discussion and limitations
Where do we go from here?

## Main ideas
### Intro (basic problems and ideas)
>"overparametrized" models actually aren't overparametrized, and generalization is not just a question of broad basins because loss basins actually aren't basins but valleys of constant, minimum loss (The higher the dimension of these minimum sets, the lower the effective dimensionality of your model.)

> Generalization is a balance between expressivity (more effective parameters) and simplicity (fewer effective parameters).

> minimum-loss sets result from the internal symmetries of NNs and from the underlying true distribution.

There are 2 types of symmetries
- *generic symmetries* predetermined by the architecture
- *non-generic symmetries*, which the model can form or break during training

The central claim is: **The presence of more complex singularities in the parameter space allows the model to implement simpler functions with a lower effective dimension, which in turn leads to better generalization ability.**

Complex Singularities ⟺ Fewer Parameters ⟺ Simpler Functions ⟺ Better Generalization
### Back to the Bayes-ics
$q(x)$, 
$p(x \mid w)$, 
$\varphi(w)$
$$
D_n = \{ X_1, \dots, X_n \}
$$




### Statistical learning theory is built on a lie
### Learning is physics with likelihoods
### Why "singular"?
### Phase transitions are singularity manipulations
### Neural networks are freaks of symmetries
### Discussion and limitations
### Where do we go from here?