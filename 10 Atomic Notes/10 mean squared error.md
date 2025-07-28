---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - MSE
  - within group variance
status: WIP
created: 2025-05-03 16:11
updated: 2025-05-03 16:10
---
---
## Overview
- MSE is a measure of the variance that remains unexplained by factors of a statistical model 
	- Can be known as random error
	- Mean Squared Error, (MSE), is the mean of the squared [[10 residuals]] in a model
	- Can be biased or not, and it's definition changes based on it's use case


**In context**:
- MSE = the variance of the error term, $e$ in a [[20 Regression MOC]]
- MSE = the within group variance of a ANOVA, as it is the variance not explained by any of the factors that we're testing within, i.e. random error
![[40 Attachments/10 mean squared error]]
	- **What the model explains:** The across group variance affects the absolute value of the the outcome, and is thus the treatment effect. And thus actually shifts the mean. 
	- **What the model doesn't explain**: Even with the treatment effect, there's a part of the model that isn't explained by the model and it's factors 

## Derivation and definition
### When Biased
- $MSE = SSE/n = \frac{1}{n} \sum_{i=1}^{n} (Y_i - \hat{Y}_i)^2$
The mean square error = the [[10 SSE]], sum of squared errors, divided by the number of variables n in the data.
- Often used in prediction (e.g. ML) where it's just a rough value that you want to minimize as a proxy to fit the best model you can
### When not Biased
- $MSE = SSE / df = \frac{1}{n-p-1} \sum_{i=1}^{n} (Y_i - \hat{Y}_i)^2$ 
	- Converges to the true **population** error variance, $\sigma^2$
	- p is the number of variables in a regression excluding the intercept. Thus n - (p+1) accounts for all terms in the regression -- such models give an unbiased estimate of the variance

## Properties
- Penalizes large errors more than small ones, due to its squared nature thus making it suitable for accounting for outliers
- 


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



