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
- remember, correlation doesn't indicate causation
- A standardised version of [[10 covariance]] that measures the **strength** and **direction** of a linear relationship between 2 variables
## measures of correlation
The correlation metric calculated between variables differs based on the type of **variable**:



 - **continuous, numeric variables** - [[10 Pearson's correlation coefficient]]
 - **binary variables** - [[10 Tetrachoric Correlation]]
 - **ordinal (ordered) variables** - [[10 Polychoric correlation]]
 - **Nominal varaibles** - [[10 Cramer's V]] (effect size); [[chi squared test]] (significance of effect)
 - **continuous & nominal**:  [[intraclass correlation]] (effect size); [[10 ANOVA]] (significance of effect)

*refer to the [[30 Statistical Tests Cheatsheet]]


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