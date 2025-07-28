---
Subjects:
  - statistics
  - causal inference
tags:
  - academics
aliases: 
status: WIP
created: 2025-06-09 17:35
updated: 2025-06-09 17:35
---
---
## Overview
- no [[10 Atomic Notes/10 confounders|omitted variable bias]]
- each predictor variable provides us with information that cannot be obtained from any **other part** of the model
	- if you leave out a confounder, it acts in your model through the error term (as it's unaccounted for)
	- e.g. $Salary = \beta_0 + \beta_1(Years\ of\ education) + \epsilon$
	- However, SES could affect both one's years of education and salary. Removing it would mean that **Years of Education** is no longer exogenous as part of the information it provides can now be obtained in the error term (as SES acts through it)


## Issues with no exogeneity (endogeneity)
- model cannot be used to infer causation, though it can still be used for predictive purposes


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



