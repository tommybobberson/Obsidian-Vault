---
Subjects:
  - causal inference
tags:
  - concept
  - definition
  - academics
aliases: 
status: WIP
---
---
# Causal notation <!-- Note title should be the precise name of the concept -->

## Summary/Definition
We'll be exploring the different terms to represent causality and association in a population/sample of interest 
	
## Explanation
Causal inference deals with investigating the effect of something (treatment here) on an outcome

Out of a sample of $n$ individuals,
$T_i$ - the [[10 treatment]] of unit $i$ 
	- binary (given or not given treatment), $T_i$ = 1 or 0
	- continuous (dosage of medicine)
	
$Y_i$ - the **observed outcome** of unit $i$ (**our variable of interest**)
	- can be binary (died or didn't ), $Y_i$ = 1 or 0
	- continuous (test score), 

Ideally, we'd want to study the whole population with and without treatment to observe $T_i$ for all $n$ individuals. However, in the real world

**it's simply impossible to give each person both treatments irl, so we make do by observing the [[10 Outcomes]] for parts of the sample that do receive each   - i can't both give and not give a guy the the treatment**  from which we can derive each individuals [[10 Outcomes|counterfactual outcomes]] 



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