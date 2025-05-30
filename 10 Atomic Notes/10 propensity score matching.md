---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
aliases:
  - ps matching
status: WIP
created: 2025-05-02 09:06
updated: 2025-05-02 09:06
---
---
## Summary
Propensity score matching is a way to estimate the treatment effect of a certain treatment (usually through logistic regression), by allocating each response/individual a propensity score based on their covariates. And matching individuals with similar propensity scores to determine the difference in treatment effects. 

This allows for the simulation of [[randomised control trials]] on [[observational studies]]

***Propensity score: ***
- *The probability of treatment assignment T = 1 or T = 0*, **given an individuals' observed covariates**
- For **treated and non treated subjects** with the same propensity score, their covariates are the same
- Sort of an index to denote the state of the covariates

***Propensity score matching***
- use [[10 Logistic Regression]] (or other methods) to estimate a propensity score -> once you have a more balanced dataset, match variables with the propensity score and find the difference in their treatment effects (using logistic regression on the matched variables)
- helps estimate the [[10 Average treatment effect on the treated|ATT]] instead of the [[10 Average treatment effect|ATE]]

**alternatives**:
Regression matching
## resources
See [[30 An Introduction to Propensity Score Methods for Reducing the Effects of Confounding in Observational Studies]]

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



