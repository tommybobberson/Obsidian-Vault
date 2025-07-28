---
tags:
  - "#course"
  - "#academics"
course: 
status: notes taken
created: 
updated:
---
# Summary
- what is a linaer regression
- characteristics of a normal distribution
- The Process (OWL) of building a statistical model
	- In summary, **given our data**, we're trying to estimate the posterior distribution of a possible model; based on domain knowledge to set the functional form of the model + the priors
	- What are the 5 steps?
# Concepts
## [[10 Atomic Notes/10 Linear Regression|linear regression]]
- A statistical golem (i.e model)
- **characteristics**:
	- geocentric: 
		- describes associations and makes predictions between variables; however, in the real world, it is always mechanistically wrong (i.e. it's much too ideal and relies on ideal assumptions)
		- What's wrong is that it isn't an accurate mechanistic model of the system that you're studying
	- gaussian:
		- linear regression is inherently gaussian, i.e. it uses the gausian error model
		- LR depends on the error model of the [[Normal distribution]] aka the gaussian distribution
- many special cases of LR like anova, ancova etc.
## [[Normal distribution]]
- many natural forces result in the normal distribution, why?:
	- Generative: summed fluctuations in nature tend towards the normal distribution (e.g. the fluctuations in the height of a population)
	- Inferential (statistical): For estimating mean and variance, the normal distribution is the most suitable to be used as it is the **least informative**; basically with the least information (only the mean and the variance), it covers the most bases and can be generalised
- variables don't have to be normally distributed for the normal model to be useful, it's just a tool to estimate _mean and variance_
- imagine coin tosses: there are many many **mroe ways** that you have a simlar number of heads and tails vs all tails or heads

## Making Geocentric models
### Steps:
1. language for representing statisical models (golems)
2. Calculate [[Posterior distributions]] with multiple unknowns
3. construct and understand (linear) models

## Owl-drawing workflow
### Steps:
1. state a clear question
2. sketch your causal assumptions (DAGs maybe)
3. Use the sketch to define a generative model (code that generates synthetic observations)
4. Use generative model to build estimator (your distributions)
	-  Profit? (evaluate whether your model actually works) if no, back to 2, if yes go on to 5
5. use your generative model to analyse your data

### Case-study, constructing a linear regression model
**Question**: Describe the association between ADULT, weight and height

**Causal Assumptions**: How does height influence wieght?
	H -> W <- Unobserved; i.e. weight is a function of height and unobserved stuff
	 $W = f(H,Unobserved)$
	 
**Defining a generative model**: What generative model shall we use?
	- **Options**: 
		1. Dynamic: incremental growth of organism; both mass and height derive from growth patterns; **the gaussian variation is a result of the summed fluctuations**
		2. static: Changes in height result in changes in weight but there's no mechanism; **Gaussian variation is a result of growth history**
	- **Proposed model**:
	  For adults, $W = \beta H + U$
		- where U and H, are normally distributed
		- U here basically becomes part of the error term
	- **How are models described?**
		- List all the variables (generative or statistical)
		- Define how each variable get's it's value, it can be a **[[deterministic function]] or [[distributional function]]** of other variables
			Deterministic: $W = \beta H + U$
			Distributional: $U_i \sim Normal(0, \sigma)$ - bascically, U is a function of sigma (the varaince) in the context of a (**normal**) distribution

**Building an estimator**: To estimate our outcome of interest (avg weight) and how it changes with height
	- **Mathematically**: $E(W_i|H_i) = \alpha + \beta H_i$ 
	- we want to define the expectation of weight for each individual height
	- **estimator of interest**: we want to build a posterior distribution
		- And the posterior distribution here gives the probability of a specific regression line (and thus the intercept and slope)
		- ![[01 Statistical Rethinking L3 17-06-25_0.excalidraw]]
		- basically we're updating our linear model, defined by the 3 unknown constants alpha, beta and sigma, (or rather the posterior for the linear model) as we run through different each set of Height and weight where $i = {1, ..., i}$
		- In the following model: the **bolder** the lines, themore likely the regression equation
		- ![[01 Statistical Rethinking L3-visualised probability distribution of linear models with different no of data points.jpg]]
		- ==the posterior defines the probability of an infinitely many number of linear regressions==
	- **ways to estimate**:
		- grid estimation: discrete number of individua
		- [[quadratic approximation]]: we approximate the posterior as a [[multivariate]] [[Normal distribution|gaussian distribution]]
			- something like $W_i ~ Normal({\mu}_i, \sigma)$
			- ==posteriors are derived from iterating over the data that you already have, so it follows that they become more accurate the greater the sample size of your current data==
			- it's called quadratic because the estimate is based purely on the variance which = $\sigma^2$
			- you must define [[prior distributions]] for these things that you want to estimate
			- ![[01 Statistical Rethinking L3-quadratic approximation.jpg|400]]
		- **how you estimate these prior predictive distributions?**:
			- priors should express scientific knowledge but **softly**, i.e. they should align with domain knowledge and be scientifically reasonable
			- in our height and weight example:
			  - $\alpha$ is centred around 0, because it **makes sense for individuals of 0 cm to be 0 kg,** and so the intercept of weight against height should be 0
			  - $\beta$: the slope of an individual's weight with their height should be somewhere **between 1 and 0, because most adults aren't the same weight (kg) as with their height (cm)**; it should also be **positive**
			  - $\sigma$: **standard deviations of weight must be positive**, so uniform(0,10) gives a sd between 0 and 10 kg between different individuals
		  - running our previous priors  we get to see the different regression lines which can be produced by our priors; **and the intercepts are quite problematic**
		  - ![[01 Statistical Rethinking L3-example of priors.jpg]]
		- **Priors**:
			- there are no correct priors, only scientifically justifiable priors (or posteriors too) -> defined by your causal model
			- priors aren't the most important in **simple models** - because you don't want to make them super strong; priors are more impactful in complex models
			- priors should never be extremely strong assumptions

**Validating our model**: 
	-Test statistical model with simulated or real observations
	- vary slope and make sure that your posterior mean tracks it?
	- use a large data sampel to see that your **estimator (the posterior)** converges to the same values

**Analysing the data**
- your parameters cannot be treated independently of one another and cannot be independently interpreted
- **push out posterior predictions** and describe your posteriors (i.e. most likely values of alpha, beta and sigma in our current example) -> basically run many posteriors (like draw out 20 samples of linear regression from your posterior)
- ![[01 Statistical Rethinking L3 17-06-25_1.excalidraw]]
# Attachment
![[01 Statistical Rethinking L3-Lecture_03-geocentric.pdf]]