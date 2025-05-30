---
tags:
  - moc
  - academics
aliases:
  - regression moc
status: WIP
created: 2025-05-02 23:16
updated: 2025-05-02 23:15
---
---
## Overview

A regression is a subset of a [[10 general linear model]]

It is a tool in quantifying (an estimate of) the relationship between dependent and independent variables. 

A regression equation takes the following format and has a few important outcomes
$Y = \beta_0 + \beta_1X + W'\delta' + \epsilon$
- Y: predicted outcome (units based on type of regression, e.g. lg odds ratio for logistic regression)
- $B_0$: Intercept of regression (no real-world significance -- the value of the outcome when all predictors = 0)
- $B_1X$: the outcome scaled by each unit / the presence of treatment
	- $B_1$: the slope of X, on outcome
	- $X$ (or $T$): the value of the treatment (or this can be any variable $X$) 

- $W'\delta$: all the other terms included in the regression (doesn't exist for [[simple linear regression]])
    - W: a vector of the other control variables included (w' because it's used in a dot product)
    - $\delta$ : a vector of the control variables' respective coefficients 

- $\epsilon$: the model error, due to additional variables that you haven't accounted for
	- in building any regression model there will always be some sort of error, as it's impossible to account for all factors (either because it's too expensive or it's not relevant enough to your variable under study to include and would result in more uncertainty instead)

- degrees of freedom:
	- p + 1, where p is the number of independent variables in the regression. 
	- +1 for the intercept
## Characteristics of regression coefficients
- **Magnitude**: The degree of change in the dependent variable for each unit change in the independent variable

- $R^2$: The proportion of variance in the dependent variable explained by each independent variable - if this adds up to 1,we are able to perfectly explain how the dependent changes with the independent variable

- p-value: tells us if we're confident of if the regression term is significant in predicting the dependent variable



## For Causal inference 
- Helps us estimate the causal effect on average, [[10 Average treatment effect|ATE]], through the ​following. 
    - if $Y_i = \beta_0 + kT_i + \epsilon$, then when $T_i$ = 1, we get $E[Y|T = 1]$ and $E[Y|T = 0]$ otherwise. 

- As we are accounting for bias(resulting in 0 [[10 selection bias]], we can derive that, with a constant treatment effect, $Y_{1i} = Y_{0i} + k$ where K is = [[10 Average treatment effect|ATE]] = $E[Y_1 - Y_0]$ = $E[Y|T=1] - E[Y|T=0]$
## Types of Regression 
The type of regression is dependent on the number and types of variables that were interested in
- [[10 Linear Regression]] 
- [[10 Logistic Regression]]
- [[10 univariate]] vs [[10 multivariate]]: single or multiple dependent (outcome) variables
- [[10 simple regression]] vs [[10 multiple regression]]: single or multiple independent (predidtor) variables

## Methods of Regression 
The Method of Regression is how the quantified estimate between variables is **calculated**
- [[OLS]]
- [[Maximum Likelihood ]]
- [[10 Weighted Regression|Weighted least squares]]
- [[10 Grouped Regression]]
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



