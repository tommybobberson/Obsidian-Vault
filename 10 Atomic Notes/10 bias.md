---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - bias
status: WIP
---
---
# bias 

The (intrinsic) difference in outcomes between populations, that do receive the treatment as compared to those that didn't, not due to the treatment. 

*(which may or may not also contribute to them being treated, and the difference in their observed outcome) 

Mathematically:
[[10 association]] 
$E[Y|T=1] - E[Y|T=0] = \underbrace{E[Y_1 - Y_0|T=1]}_{ATT} + \underbrace{\{ E[Y_0|T=1] - E[Y_0|T=0] \}}_{BIAS}$
## When association is causation 
When bias = 0, [[10 association|Association]] = [[10 causation]]. which also means that 
- $E[Y_0| T = 0] = E[Y_0| T =1]$, where there ar no intrinsic differences between the to be treated and untreated populations 
- in such cases, the differences in expected means, becomes the causal effect; [[ATT]] = [[ATE]]

**Types**:
[[10 selection bias]]: occurs when you condition on a collider variable between your explanatory variable and independent variable
[[10 confounders|confounding]] bias: occurs when you fail to control for the confounder or open up more backdoor paths
[[10 confounders|omitted variable bias]]


## Examples
### Example 1
 

If the outcome is survival, it may be the case that when comparing those wgo received treatment (expensive chemotherapy) and those who didn't receive treatment, the for those who Y = 1,they had better healthcare as they could afford better diets, are located in richer areas where there are better doctors etc. As such, their increased rate of survival isn't necessarily due to the treatment even though it may seem so. (if you gave the poor the treatment too they may not get better at all given that they have a lower baseline level of health)

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