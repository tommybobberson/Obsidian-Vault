---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# correlation 
- remember, correlation doesn't indicate causation; correlation coefficients **must be examined in conjunction with graphical plots of the data itself, as a high correlation coefficient doesn't necessarily mean it's a linear relationship r/s**
- A standardised version of [[10 covariance]] that measures the **strength** and **direction** of a linear relationship between 2 variables
	- sign measures direction
	- magnitude measures strength

- correlation is ==the covariance between the standardised variables== OR ==**the ratio of the covariance to the [[standard error|standard deviations]] of the 2 variables**==
- $$Cor(x,y) = \frac{Cov(x,y)}{s_x s_y}$$
- **cannot be used for prediction**, as correlation coefficient only holds true based on the data it's been given

## Properties
- symmetric, $Cor(X,Y) = Cor(Y,X)$
- scale invariant, unlike [[10 covariance]]
- $-1 \leq Cor(X,Y) \leq 1$
- **can only measure ==linear== relationships just like [[10 covariance]]**
	- as such, $Cov(X,Y) = 0$ doesn't indicate there's no relationship between X and Y but rather that there is no measurable linear relationship
- can be heavily influenced by [[outliers]], refer to [[Anscombe's quartet]]

## measures of correlation
The correlation metric calculated between variables differs based on the type of **variable**:



 - **continuous, numeric variables** - [[10 Pearson's correlation coefficient]]
 - **binary variables** - [[10 Tetrachoric Correlation]]
 - **ordinal (ordered) variables** - [[10 Polychoric correlation]]
 - **Nominal varaibles** - [[10 Cramer's V]] (effect size); [[chi squared test]] (significance of effect)
 - **continuous & nominal**:  [[intraclass correlation]] (effect size); [[10 ANOVA]] (significance of effect)

*refer to the [[38 Statistical Tests Cheatsheet]]


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