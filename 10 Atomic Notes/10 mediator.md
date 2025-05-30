---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - Mediator
status: WIP
---
---
# mediator 
A mediator variable is a variable through which the causal effect flows, lying on the [[10 paths|dependency path]] 

In other words, a mediator accounts for the relationship between your dependent variable and independent variable of interest

B is a mediator
![[10 Causal relationships 2025-04-23 18.33.56.excalidraw]]

**types**:
- partial mediation - the mediator explains some of the relationship between A and C
- full mediation - the mediator explains all of the r/s between A and C, when it is controlled for, they are [[10 conditional independence|conditionally independent]], the causal path is [[10 blocked|block]]

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