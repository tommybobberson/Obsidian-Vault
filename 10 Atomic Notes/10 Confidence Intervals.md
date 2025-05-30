---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - CIs
  - confidence interval
  - credible interval
status: WIP
---
---
# Confidence Intervals 
[[frequentist]]
- Defined in the context of hypothesis testing, the 95% confidence interval is such that we can be 95% confident that the true (**unknown estimate**) lies within the limits of the interval, based on **hypothetical repeats** of the same experiment
- Or, given that the **value of the confidence interval itself** is also normally distributed, constructing multiple CIs with multiple repeated experiments, 95% of the constructed intervals will include the true value of the parameter
[[bayesian]]
- denoted as a credible interval
	- an interval for which there is a **95%** probability the true parameter lies given the observed data


## Use cases 
- include in plots when **you want to emphasise** the uncertainties within the data 
      - (small sample sizes where you feel like the proportions plotted and visualised aren’t representative of the relationship you want to convey
      - Bar plots or dot plots with low sample sizes 
## methods of calculation
- Wald
- Agresti-coull
## R 
- `library(binom)`



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