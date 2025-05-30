---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - 2-factor anova
status: WIP
created: 2025-05-19 11:16
updated: 2025-05-19 11:16
---
---
## Overview
Different from the one-way ANOVA, in that you want to compare the effect of 2 or more variables on a dependent variable. **And** test for any possible interactions between the 2 factors.

e.g. You want to test how different amounts of fertilizer A and fertilizer B affect the growth of a plant. And how they interact

- A factorial experiment is conducted (i.e. experiments with different levels each factor)

**What you can test for**:
1. Main effects (of A or B on the dependent variable itself)
2. Interaction effects (how A affects B on dependent)


## Notation
A: factor A
B: factor B
k: number of levels of factor A
l: number of levels of factor B
kl: total possible treatment combinations
n: number of observations per treatment 

[[SSE]]: sum of square errors
[[MSE]]: mean square error, or the best estimate of $\sigma^2$ in the context of a 2 way anova
## Assumptions
- **within group variances are the same**: Observations (between different groups) of a particular treatment are independently selected from a normal distribution with variance $\sigma^2$ (which translates to $SS_E$)
- samples from different treatments are independent 
- **balance design** (nice to have but not necessary): an equal number of observations in each treatment increases the power of the test

## Intuition
As in a [[One way ANOVA]], you seek to breakdown the total sums of square (and variance) down into that due to treatment and random variation. Here your F-statistic is given by $MSE_{treatment}/MSE_E$

$SS_{total} = SS_{treatment} + SS_{E}$

In a 2-way ANOVA we determine the sum of squares (and thus the variance) in the dependent variable that is explained by each level of treatment, random error and the interaction effect. 

**Aim**: 
	to determine if the shift in the means is substantial enough, as compared to the variance within the group. To reflect a statistically significant shift (and thus treatment effect)
	
	Our null, starts off assuming that the treatment outcomes with each factor are drawn from the same distribution
	

$SS_{total} = SS_A + SS_B + SS_{AB} + SS_E$

Where:
$$SS_{total} = total \ sum \ of \ squares;\ df: kln$$
$$SS_A = Sum \ of\ squares\ of \ the \ main \ effect \ of factor \ A; df = k-1$$
$$SS_B = sum\ of\ squares\ of\ the\ main\ effect\ of\ factor\ B; df = l-1$$
$$SS_{AB} = sum\ of\ squares\ of\ the\ interaction; df = (k-1)(l-1)$$
$$SS_E = the\ error\ sum\ of\ squares\ (within\ group\ sum\ of\ squares); df = kl(n-1)$$

And subsequently, to compare the ratio of the [[10 mean squared error|MSE]]s of A to E, B to E and AB to E

Where the MSEs of A, B and AB represent the across group variance between groups A, B and AB. Thus, acting as a proxy for the treatment effect (i.e. how much the group means shift)

Here the orange and Green groups represent the distributions and means for the dependent variable given any 2 variables. 
![[30 Analyzing multivariate data 2025-05-19 01.26.58.excalidraw]]
- If there is a difference in treatment effects, the across group variance becomes much larger than the within group variance. (of both factors, cause they have the same variance) And thus, we can conclude that it's unlikely there isn't a real difference in the means of the 2 treatment levels (and that it's due to within group variance)

## Hypotheses testing
There are 2 levels of hypothesis testing in a 2-way anova. Testing for interaction between treatment levels and for the treatment effect of each factor.

	**the presence of an interaction preculudes testing for treatment effects of each individual variable**

![[10 Two way ANOVA 2025-05-19 12.32.23.excalidraw|800]]

**Interaction**
$H_0:$ There is no interaction between the factors
$H_1$: There is interaction between the factors

**Treatment effects**:
$H_0$: There is no effect of Factor A on the response variable
$H_1$: There is an effect of factor A on the response variable

$H_0$: There is no effect of Factor B on the response variable
$H_1$: There is an effect of factor B on the response variable

## Steps:
(manually)
1. calculate the SSEs for each hypothesis that you're testing for
2. Calculate the  number of degrees of freedom of each level
3. Calculate the MSEs of each factor
4. Calculate the F-statistic for each hypothesis
5. Conduct hypothesis tests to see if the alternative hypothesis is significant, in the following order:
	1. Interaction between A and B, A * B
	2. Main effects of A and B

Each step can be stored in a 2-factor ANOVA table as shown below
![[10 Two way ANOVA 2025-05-19 12.47.31.excalidraw|700]]

---
#### Linked Concepts (Auto-Generated)
```dataviewjs
// Requires Dataview plugin. Lists outgoing links from this note's body
// that likely point to other Atomic Notes (by checking the path).
const outlinks = dv.current().file.outlinks;
// Filter for links pointing to the '10 Atomic Notes' folder (adjust path if needed)
const conceptLinks = outlinks.filter(link => link.path.startsWith("10 Atomic Notes/"));
if (conceptLinks.length > 0) {
    dv.list(conceptLinks);
} else {
    dv.paragraph("No links to other Atomic Notes detected in the body.");
}
```



