---
tags:
  - "#course"
  - "#academics"
course: statistical rethinking 2023
status: notes taken
created: 2025-06-03T20:00:00
updated: 2025-06-03T20:00:00
---
# Summary
- What is [[Bayesian Data Analysis?]]
	- find explanations/assumptions that are the most plausible, given your data
	- It gives you no guarantees except that it's logical. It can't tell you what's actually happening in the world but, given the correct inputs and causality, you get to estimate something according to your subjective beliefs as best as possible
- What are the components of Bayesian data analysis
- What are the assumptions and characteristics of bayesian data analysis
- How? do you carry out bayesian data analysis, what's a workflow that you should follow
- ==What is the framework for going from a scientific question to a bayesian causal model==

# Concepts
## Building a Bayesian Model
1. Define a generative model: 
   how are you gonna get your data
2. define a specific [[estimand]]
3. design a statistical way to produe an estimate
4. test (3) using (1)
5. Analyse the sample and summarise
### 1. building a bayesian model
- Consider the causal relationships between the variables you want to study
	- your variables and statistical analyses should always be built off domain knowledge and [[10 causation|Causality]]
	- this helps you consider what variables you need to include and or what relationships you need to study
	- using tools like [[DAG]]s
### 2. Define a specific estimand
- What is the outcome that you want to study
- using our example below, let's define it as the combination of blue and white faces obtained upon doing a dice roll



## 3. design a statistical way to produce an estimate
- the idea is to create a measure which represents the probability of smth happening -- we're using the relative frequency of an event happening
### What is Bayesian data analysis
- Looking at the probability of what happened given what **could've happened**, given an assumption about the data  aka [[prior]]
	- for each possible explanation (scenario of the outcome) -> consider the combinations of events that result in this -> consider their relative probability
	- **Example**: we have a four sided die whose sides can take on either blue or white. 
	- We want to observe the **likelihood of seeing blue, white then blue in our first 3 rolls**
	 ![[01 Statistical Rethinking Lecture 2-dice bayesian example]]
	- The likelihood of observing this is based on the actual composition of the dice 
	![[01 Statistical Rethinking L2 03-06-25.excalidraw]]- when there are 3 blue sides on the dice, there are 3x1x3 ways to get the "bwb" outcome
	- when there is only 1 blue side on the dice, there are 1 x 3 x 1 way to observe the "bwb" outcome
		
- **things that can happen in more ways are more plausible**, and probabilities are represented by the relative frequencies of things happening
	- ![[01 Statistical Rethinking L2-combinations of observed dice rolls.jpg|400]]
	- The possibilities represent the possible combinations of faces that the dice can have, as shown by the possible combinations:
	- ![[01 Statistical Rethinking Lecture 2-combinations of dice rolls|400|1303]]

- [[Probability|Probabilities]] can be updated as we continuously sample, conditional on the state of our current observations. And the  probabilities of an event happening, in light of the data are known as the [[Posterior distribution]]. 
- Your posterior's shape which defines the relative probabilities of things happening changes as you get more and more data
	![[01 Statistical Rethinking Lecture 2-Posteriors and priors|533]]

## 4. Test before you estimate
- Code a generative simulation and estimator
- test your estimator with the generative simulation
- with our previous example, we can simulate tosses, whilst inputting the number of blue and white faces on the dice which we want -> and make sure that we don't get weird results


## What happens for a dice with an increasign number of sides
![[01 Statistical Rethinking L2-probabilities of dice combinations with varying faces.jpg]]
we get different posteriors
- all bars are getting shorter, as each bar represents a smaller relative probability
- in tu9s case the posterior is proportional to $p^W(1-p)^L$

## [[Beta distribution]]
- getting [[normalised]] probabilities
![[01 Statistical Rethinking L2-Beta distribution.jpg]]
- the relative number of ways shapes the posterior


## Characteristics of Bayesian Inference

1. There is no minimal sample size
2. Shape embodies the sample size 
3. There are no point estimates (i.e. you cannot say that the probability of something happening is the relative density). What we're interested in is the posterior distribution itself
4. There is no one true confidence interval
	- there's nothing special about different [[certainty intervals]] like 95%,99% etc. Because if you think about it, nothing magical happens at the boundaries of the intervals
	- Also where the posterior distribution itself is of concern, the X% CI can just be moved around under the posterior to cover the required area

## 5. Analyze the sample and summarise
- the implications of the model depend upon the **entire posterior distribution**
- We must average any observation over the whole posterior distribution
- this can be done without using integral calculus by sampling the posterior
### what do you want to calculate from your posterior?
- you can calculate what would have happened in other cases, e.g. when you have sampled something 100 times, 1000 times, 50000 times etc.?
![[01 Statistical Rethinking L2 03-06-25_0.excalidraw]]
- ==follow up on this, idk what these mean==

### Things we'll calculate with samples in this course
- model based forecasts
- Causal effects
- [[10 Outcomes|counterfactual outcomes]]
- Prior predictions![[01 Statistical Rethinking L2-Lecture_02.pdf]]