# Summary of Dialogue introduction to Singular Learning Theory
by Olli Järviniemi
[link](https://www.lesswrong.com/posts/CmcarN6fGgTGwGuFp/dialogue-introduction-to-singular-learning-theory)



This post is a dialogue between two characters, Alice and Bob, intended as a (somewhat self-contained) introduction to Singular Learning Theory (SLT) for non-specialists.


## TL;DR

SLT is an approach to better understand how models learn by analyzing the learning process, not just its final outcome.

SLT proposes a Bayesian-physical paradigm for learning, using tools like Bayesian updates and the concept of free energy.

At the core of the theory are singularities: regions in the function space where different parameters can define the same function. SLT suggests that singularities are the key to understanding generalization and model behavior.

SLT is the theory underlying developmental interpretability. Unlike the mechanistic approach, it studies the model's training process rather than the finished model. SLT examines the geometry of the loss landscape, where singularities cause phase transitions. This approach posits that emergent abilities are a macro-level consequence of these phase transitions. Therefore, the ability to predict phase transitions could allow us to foresee the emergence of new model capabilities.

### Questions This Post Answers
**Q: What does SLT study?**

**A:** How the model develops during training.

SLT attempts to map (1) the measurable properties of models that we can observe and simulate to (2) the high-level behavioral properties we sometimes discover in models post-facto (often to our surprise). The ultimate goal is to use a model of the development of measurable properties (1) to predict the real high-level properties (2), ideally before training even begins.

The summary is divided into two parts, mirroring the structure of the original article:

- Part 1: Theoretical Foundations

- Part 2: Practical Side

### Part 1: Theoretical Foundations
**Q: How does the Bayesian setting differ from gradient descent? And what is it, anyway?**

**A:** Bayesian inference provides a formal framework for understanding what "learning" is.

The Bayesian method considers all possible model parameters, assigns them a prior probability, and then updates these probabilities based on data. Although this method is computationally expensive, it provides a cleaner foundation for theoretical analysis.

Gradient Descent (GD) approaches start with some (e.g., random non-zero) parameter values and then, at each step of the GD algorithm, slightly modify these values based on the training data to arrive at a single, sufficiently good set of parameters. Bayesian inference, in contrast, considers a probability distribution over all possible parameter sets and shifts this distribution based on training data, assigning higher probabilities to better parameter sets.

**Q: What are phase transitions and where do they come from?**
**A:** The core idea is that the naive notion of gradual convergence is definitively wrong. The post gives an example of distributions over 10k training examples, 10k + 500, and (10k + 500) + another 500, which differ qualitatively. Such abrupt jumps are called phase transitions.

Phase transitions are sharp, qualitative shifts in a model's behavior during training. They are caused by a trade-off between two archetypal classes of models that can exist in the parameter space:

Mediocre but robust models: These correspond to wide, low "hills" in the likelihood landscape. The parameters are resistant to small perturbations, meaning many similar parameter settings yield comparable, albeit mediocre, results.

Excellent but fragile models: These correspond to narrow, high "peaks" in the likelihood landscape. They achieve excellent performance on the training data but only for a very precise and narrow range of parameter settings.

**Q: How do you calculate the number of "similarly accurate" models?**
**A:** In the Bayesian approach, we're not just interested in finding the highest point (the model with maximum performance) but in estimating the total probability of an entire region in the model space. The volume of a region is roughly its height × width.

A narrow peak might lose out to a wide hill with a small amount of data. However, as more confirming evidence accumulates, its volume grows, leading to a phase transition. This is empirically confirmed in neural networks, where flat minima are found to generalize better than sharp ones.

So, when a model receives new data and performs a Bayesian update, it doesn't just look for a higher peak. It re-evaluates the volumes of all regions. SLT formalizes this mathematically by introducing the real log-canonical threshold (RLCT), which characterizes the geometry (width and complexity) of these regions.

**Q: Why is the theory called "singular"?**
**A:** The concept of "singularity" in SLT refers to the geometry of the loss landscape. The key idea is that the "volume" of models that perform equally well is crucial. Models in "singular" regions, which have a smaller "learning coefficient" (a measure of volume expansion), are more likely to be selected in a Bayesian framework because they represent a larger mass of equally performing models.

**Q: What does the loss landscape have to do with it?**
**A:** A key feature of SLT is its consideration of the shape and "singularity" of parameter regions. In real-world problems, loss function minima are often not simple parabolas; their geometry can significantly affect the volume of near-optimal solutions and, consequently, the model's selection. This relationship is described by the learning coefficient, which influences the model's Bayesian probability.

### Part 2: The Practical Side
**Q: Are the conclusions from SLT applicable to models trained with variants of GD?**
**A:** There is growing evidence suggesting that the dynamics of SGD are influenced by the same geometric properties of the loss landscape that SLT analyzes. While the connection is not yet fully formalized, research indicates that the minima found by SGD often coincide with the singular regions favored by Bayesian inference.

**Q: What research provides evidence for the utility or applicability of SLT?**
**A:**

One study showed that sharp drops in loss during SGD training correspond to the phase transitions predicted by Bayesian learning. The paper "Dynamical versus Bayesian Phase Transitions in a Toy Model of Superposition" compares Bayesian-predicted phase transitions with those observed in real training dynamics, providing evidence that SLT can predict phase transitions in real models.

Another example demonstrated that the learning coefficient can distinguish between models that generalize and those that simply memorize data.

**Q: What predictions does SLT make?**
**A:**

Prediction about Phase Transitions: Since GD doesn't explore the entire parameter space, some phase transitions predicted within the Bayesian SLT paradigm won't occur during the training of a real model using GD methods. However, SLT makes a testable prediction: for any observed phase transition, there is a "Bayesian reason." This means one can predict all possible phase transitions, and some of them will happen to the real model. Furthermore, everything that happens to the real model will have been predicted if you've mapped out all the phase transitions in the Bayesian setting. This is a strong version of the claim, made in an idealized world, with reality introducing its usual adjustments.

Theoretical Justification for Double Descent: While double descent was identified empirically before developmental interpretability began making predictions, the theory predicts that such a phenomenon will occur, and we know it does.

**Q: What are the open problems and future research directions in SLT?**
**A:** The main ones are:

- A more rigorous extension of SLT to non-Bayesian settings.

- Understanding the role of optimization algorithms (e.g., specific GD implementations) in finding singular points.

- Applying SLT to more complex and realistic neural network architectures.

### Comments on the Post
**Q: What is the main criticism of SLT?**
**A:** The primary criticism of SLT is its extreme mathematical complexity, which makes its direct application to real-world problems difficult. Additionally, it is an asymptotic theory, meaning it describes the behavior of models as the amount of data approaches infinity, and its assumptions may not always hold for real models or finite datasets.