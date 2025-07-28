---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
  - guide
aliases:
  - ps matching
status: WIP
created: 2025-05-02 09:06
updated: 2025-05-02 09:06
---
---
## Summary
Propensity score matching is a, [[10 Propensity Score]] method, to estimate the treatment effect of a certain treatment by matching individuals who were treated and untreated (T = 1 and T = 0) who have similar covariates. This tackles the issue of how, in non-RCTs, individuals who were treated / chose to take on the treatment have factors that influence their decision to choose the treatment and the indepednent variable of interest.

This is done by allocating each response/individual a propensity score based on their covariates. And matching individuals with similar propensity scores to determine the difference in treatment effects. 

This allows for the simulation of [[randomised control trials]] on [[observational studies]]

==Estimates the [[ATT]] instead of the [[ATE]]==

Mathematically A propensity score is defined as probability that an individual receives the treatment given a set of observed covariates.$$e(X)=P(T=1∣X)$$
## Steps

1. ***Model the Propensity score:***
- *The probability of treatment assignment T = 1 or T = 0*, **given an individuals' observed covariates**
- For **treated and non treated subjects** with the same propensity score, their covariates are the same
- Sort of an index to denote the state of the covariates
- ==it is basically the odds ratio (or in rare cases of a continuous treatment) of an individual getting the treatment, and you want to match individuals who are as likely to get the treatment.
- **derivation**: typically by running a [[10 Logistic Regression]] where the independent variable is the OR of you getting treated (binary treatment, T= 1 or 0), and the dependent variables are your covariates
$$log(\frac{e(x)}{1−e(X)})=β0​+β1​X1​+β2​X2​+…+β_k​X_k​$$

Where:

- 𝑋𝑖 are covariates (e.g., age, income).
- 𝛽𝑖 are coefficients estimated from the data.



2. ***Match the individuals***
-  match individuals with similar propensity scores and find the difference in their treatment effects (using logistic regression on the matched variables)
- **matching methods:**
	  - greedy matching
	  - nearest neighbour matching
- **take note**:
	  - ideally you want to have many variables matched?

3. ***Check the balance of covariates***
- evaluate whether the matched groups have similar [[10 covariance|covariate]] distributions
- the whole point of propensity score matching is to compare the effect of treatment on individuals with a similar background. However, it's possible that the logistic regression (or other method) that generated the propensity score allowed different sets of variables to produce the same propensity score, given it is just a measure of the likelihood of being treated. **A causal structure which could result in this is as follows:**
![[10 propensity score matching 18-07-25_1.excalidraw|500]]

4. ***Estimate Treatment Effect***
- The differences in the outcome variable between matched variables is the [[10 Average treatment effect on the treated|ATT]] instead of the [[10 Average treatment effect|ATE]] - given you're comparing pairs which are all equally likely to have been treated.
- Compare the average outcome (if continuous outcome) or proportions of individuals with each outcome (if binary outcome), of the **treated group against the matched, untreated group** to get the [[10 Average treatment effect on the treated|ATT]]

![[10 propensity score matching 18-07-25_0.excalidraw|600]]



## Pros and cons
**pros**:
- more statistically intuitive and easier to implement/interpret
- doesn't require exact matching on all variables
- Reduces selection bias due to observable covariates

**cons**:
- cannot account for [[10 Atomic Notes/10 confounders|omitted variable bias]], that must be tackled through [[10 instrumental variables]]
- can't account for the causal effect of covariates (unlike regression)
- loss of sample size as matching can result in a loss of unmatched units
- depends heavily on the validity of your logistic model 
- can't be used where there **are not overlaps between your treated and untreated samples**
## Alternatives
- [[regression]]


## resources
See [[38 An Introduction to Propensity Score Methods for Reducing the Effects of Confounding in Observational Studies]]

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



