---
Subjects:
  - statistics
tags:
  - academics
  - concept
aliases:
  - ordinary least squares
status: WIP
created: 2025-06-09 15:59
updated: 2025-06-09 15:58
---
---
## Summary
- what is ordinary least squares

## Overview
Ordinary least squares is a [[10 parameter estimation]] technique that is used to fit a [[20 Regression MOC]] by minimising the [[MSE|mean squared error]] between observed values, $Y_i$ and predicted values, $\hat{Y_i}$


![[10 OLS-OLS example.jpg]]
 - where the vertical lines represent the [[10 residuals]]. 
 - Essentially we want to estimate parameters to minimize the **(average of) the sum of these black lines squared**, which are the errors that we can associate with uncertainty

## Assumptions
1. no [[10 collinearity]] except in the case of confounding
	- different variables tell the same story, it becomes hard for the model to determine which variable actually caused which change
	- When they're collinear, holding one value constant limits the range of the other variable it's collinear with, e.g. height and weight. Thus reducing the reliability of your predictor coefficients
	- can't be fixed by adding an [[effect modification|interaction term]]

2.  linearity: there is a linear relationship between the dependent and independent variable
3. [[10 Normality of Errors]]: The residuals are normally distribued (plot histogram of residuals)
	- considered a weak assumption and can be ignored/less impactful when you have a great number of observations due to the CLT
4. [[10 Homoscedastic]] (have a constant variance for all values of the variable) 
5.  no [[10 auto-correlated|autocorrelation]]: Observations are independent of each other
6.  [[10 exogenity]]: 
	- There is no [[10 Atomic Notes/10 confounders|confounding]] that is unaccounted for
	- or [[10 instrumental variables]] are used
## Properties
***Advantages***: 

## Minimizing MSE

Where $\beta^*$ is a vector of coefficients (basically a coefficient for each variable X), and you want to obtain the value of $beta$ that minimises the MSE
	- $\beta^* =\underset{\beta}{argmin} \ E[(Y_i - X_i'\beta)^2]$ 
By differentiating, and equating to 0,
$\hat{\beta} = (X'X)^{-1}X' Y$, where X' is the transpose of the vector X

Thus, for each individual variable, when minimizing MSE
$\hat{\beta} = (X'X)^{-1}X' Y$



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



