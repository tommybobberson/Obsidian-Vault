---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
aliases:
  - Association
status: WIP
---
---
# association 
not [[10 causation]] 
$E[Y|T = 1] - E[Y|T = 0]$

The difference in the average outcome of those who were actually given the treatment (T = 1) and those who weren't given the treatment (T = 0)

- what we can actually observe on a real world population 

- can be used to calculate causation by accounting for the [[10 bias]]
- association is only causation when bias = 0

**transforming association to calculate bias**
given that we can only observe the treated outcome for the treated and the untreated outcome for the untreated, association can be :
$E[Y|T=1] - E[Y|T=0] = E[Y_1|T=1] - E[Y_0|T=0]$
upon adding and subtracting $E[Y_0|T=1]$

we get this $E[Y|T=1] - E[Y|T=0] = \underbrace{E[Y_1 - Y_0|T=1]}_{ATT} + \underbrace{\{ E[Y_0|T=1] - E[Y_0|T=0] \}}_{BIAS}$

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