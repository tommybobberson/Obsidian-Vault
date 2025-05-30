---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - ATT
status: WIP
---
# Average treatment effect on the treated 

Defined as the [[ATE]] for a group which was treated (where the whole group has T = 1) (can also be the converse where all T = 0) 

$ATT = E[Y_1 - Y_0 | T = 1]$

if you knew

Basically ATE by treatment group because if you knew both $Y_1$ and $Y_0$ for the treatment group that's like an ideal clinical trial where you know both possible outcomes even when you treat so you can calculate causality - this is still impossible to observe given that you only know the outcome for the treatment which that group received, i.e. when T =1 you only know $Y_1$ and when T = 0 you only know $Y_0$ 


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