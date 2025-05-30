---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases:
  - dummy regression
status: WIP
created: 2025-05-14 02:27
updated: 2025-05-14 02:27
---
---
## Overview
**Grouped regression calculates seperate regressions with ==distinct coefficients for each subgroup== within the data**.

It is _Not_ reducing a continuous variable by intervals and calculating 1 overall regression coefficient. That is [[data binning]]

It also breaks variables down into subgroups, effectively: 
**(1) reducing the number of total groups** 
or 
**(2) turning continuous variables into categorical variables** and this is achieved by 
**(3) Creating [[10 dummy variables]] for each group** 

## Aim
1.  test if there's a difference between the groups - if no their coefficients should be the same 
2.  investigate effect modification  - if the same, the slope (not necessarily the position) of the regression lines will be identical 
## Process and use cases
1. Define subgroups according to domain knowledge / any sort of significance you'd like to investigate 
2. Create dummy variables for each group 

![[10 Grouped Regression 2025-05-14 18.40.19.excalidraw]]

With this, you can investigate how different races affect a child's height on top of other factors like age and sex etc, calculating a coefficient for each race
## Benefits
- More observations per group, results in more accurate data as compared to more finely allocated groups (e.g. ages 1, 2, 3, 4 ... 18 vs ages 1-6, 6-12, 13-18)
- Allows you to capture [[10 effect modification]] (interactions) between different subgroups of the data and the dependent variable
- reduces [[variance]] **within groups**, recall as n increases, $\sigma^2/ n$ decreases (relative to a continuous variable)

## Trade-offs

- increases variances of the **coefficient estimates**, as:
	- we are estimating the effect off of a smaller sample size per group (vs the whole sample size when we were dealing with a continuous variable). 
	- and our model cannot account for the residual variance within each group -- that arises from the loss of continuous information (e.g. in a group 20-30 years old, we aren't capturing the differences between 22 and 29 year olds when we could've if we were treating age as a continuous variable), it's instead averaged out
- **reduces [[10 power]]** of the **coefficient estimates** and increases [[statistical errors]]
	- The standard error of the coefficient estimate is inversely related to the square of the number of observations in a group, $SE(β^{hat}​)= \sigma/\sqrt{n}$
	- As n drops, [[standard error]] increases, [[10 Confidence Intervals]] widen
	- widened Confidence intervals lower the probability of us rejecting a false null hypothesis (as it might now fall within our CIs), thus lowering statistical power


## Example
Perhaps you want to quantify the effect of age on vaccination uptake for children under 18 years old.
- However, taking the absolute precise age (down to the day) for each child would result in too many differing groups per se. 
- Also, vaccination trends might change with different periods of schooling

So you group these children into distinct age categories and estimate how being in these age categories affects vaccination uptake instead (rather than estimating how a 1 year increase in age affects vaccination uptake):
- Pre school (0-5 y/o)
- Primary school (6-11 y/o)
- Secondary school (12-18 y/o)

**outcome**: 
- each group is made of more data points
- you can identify the different trends in vaccination uptake unique to different age groups. Maybe vaccination rises for pre-schoolers, dips for primary schoolers and rises for secondary schoolers again. A linear regression can't capture this U shaped relationship! (and this could warrant further research)
![[10 Grouped Regression 2025-05-14 02.52.34.excalidraw]]


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



