---
tags:
  - "#course"
  - "#academics"
course: 
status: unread/notes taken/processed
created: 
updated:
---
# Summary

# Concepts
**We will cover**
- ==how to draw== models with multiple estimands, and thus processing many different models
- how to interpret the results of statistical models, and how we can look for our particular estimand of interest
- categorical variables
- splines and other additive structures

## Categorical Variables
- causes that we want to investigate which aren't continuous
- **types**: discrete, unordered types
- ==we want to build statistical models (i.e. fit a regression line) for each category

### Steps in including categorical variables
1. consider the causal relationships between our variables
   example, we want to investigate how height varies with weight. With the addition of sex

![[01 Statistical Rethinking L4-categorical scatterplot.jpg]]
2. define which causal relationships are in play
	- here we can see that height weight are both dependent on sex
	- ![[01 Statistical Rethinking L4-distribtuion of heigh and weight with sex|799]]
	- remember that there are ==unobserved causes==
		- ignorable unless they are shared among the measured variables
		![[01 Statistical Rethinking L4-DAG Sex, height, weight, unobserved.jpg]]
		- Example, of non-ignorable unobserved causes
# Attachment

