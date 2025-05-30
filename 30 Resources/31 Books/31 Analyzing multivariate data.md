---
status: reference
tags:
  - book
  - resource
aliases: 
URL/DOI: The phsyical book in your bag
Subjects:
  - causal inference
  - statistics
created: 2025-05-15 17:05
updated: 2025-05-15 17:05
---
---
# Analysing Multivariate Data

## Chapters
### Chapter 11 Analysis of Variance
A special case of the general linear regression model.
#### Use case
- To test whether a particular factor (treatment) has an effect on the dependent variable of interest
	- only notes difference but doesn't quantify the magnitude or direction of difference
- Continuous dependent variable and discrete independent variables

#### Variants:
- ANOVA: single continuous dependent, discrete indepedendent
- ANCOVA: single continuous dependent, discrete and continuous independent
- MANOVA: multiple continuous dependent, discrete independent
- MANCOVA: multiple continuous dependent, continuous independent

#### Theory behind ANOVA
**Intuition**:
We make an inference about if there's a difference between group means by comparing different estimates of the [[10 variance]] associated with these observations (within and across group)
![[30 Analyzing multivariate data 2025-05-15 17.21.18.excalidraw|700]]
### Terms of an ANOVA
#### Single factor anova
**m**: treatment levels
****$n_j$**: number of observations per treatment level
**n**: total number of observations
**$s^2_w$:** within group variances
**$s^2_a$**: across group variances
$Y_j$: group mean
$Y$: total mean
**$Y_{ij}$**: value of a variable within a group

**Anova table**:

| Source                | Sum of squares                                         | degrees of freedom                                           | Mean square                                          | F-value       | PR > F  |
| --------------------- | ------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------------- | ------------- | ------- |
| across group variance | sum of squares of group means around the overall mean. | m-1 (number of groups - 1)                                   | sum of squares / degrees of freedom (gives  $S^2_A$) | $S^2_A/S^2_W$ | p-value |
| within group variance | sum of all within group sample variances.              | n -m (total number of observations - total number of groups) | sum of squares / degrees of freedom (gives  $S^2_W$) |               |         |
| total group variance  | across group variance + within group variance          | m -1 + n - m                                                 |                                                      |               |         |


**Hypotheses**
In an anova you're just testing if there's a difference or not.
**hypothesis of no effect/null hypothesis**
$H_0: \mu_1 = \mu_2 =... \mu_m$ , this translates to identical within group variances

**Assumptions of the null hypothesis**
You aren't testing if the sample means are the same. Rather, you're testing if the sample variance between the groups / the sample variance within groups is large enough to not be up to random chance
- The total sum of squares, is equal to the Sum of squares across-groups plus the within-group sum of squares
	**Within group variances**:
	- Across all groups, the variance of observations in each group around each group mean is equal (i.e the distributions have the same shape?)
	- total degrees of freedom across groups = n - m
	- [[Within Group variance]] (and Sd) is constant, i.e. they exhibit [[10 Homoscedastic|homoscedasticity]]
	- ![[30 Analyzing multivariate data 2025-05-15 18.03.46.excalidraw]]
	- Where the within group variances are equal, $\sigma_1^2 = \sigma_2^2 = ... = \sigma_m^2$
	**across group variances**:
	-$S^2_A$ is an unbiased estimate of $\sigma^2$ when $H_0$ is true, but not when it is false
	- degrees of freedom = (m-1) i.e. one for each of the group means
	- When the null is false, the estimate of $S^2_A$ reflects the variability due to sampling error **AND** the systematic differences due to the presence of **treatment effects**

**alternative hypothesis is true**
- using a [[f-test]], the ratio between $s^2_a / s^2_w$ will **significantly** differ from 1
- the across and within group variances are significantly different
- degrees of freedom for the f test are m -1 and n - m
- the f-statistic gives a p-value to reject if the within and across group differences differ at each x-level of significance
	- It basically tests if the across group variances ae too far out from the within group variances such that it's not feasible for it to exist 
	![[30 Analyzing multivariate data 2025-05-19 01.26.58.excalidraw]]

#### Two factor anova
- 


## Related Resources


## Attachment

