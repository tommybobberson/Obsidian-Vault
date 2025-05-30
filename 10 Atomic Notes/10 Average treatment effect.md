---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - ATE
---
# Average treatment effect 

$ATE = E[Y_1 - Y_0]$

Formally, it is the sum of all [[10 individual treatment effect]]s divided by the population, an average effect 

- still this is impossible to observe because we need to know all the individual treatment effects and thus both outcomes for each individual
- this is not (in a)real population the average outcome of the treated - the average outcome of the untreated. **this implies association = causation**

However we can calculate the [[10 Average treatment effect on the treated]]
## Summary/Definition

## Explanation

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