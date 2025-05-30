---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - path
  - dependency path
status: WIP
---
---
# paths 
if dependency flow is water, paths are the pipes through which they flow

Refers to the flow of dependency from one variable to another as drawn out by combinations of [[10 edges]] and [[10 Nodes]] which formm different [[10 Causal Structures]]
- can be open or closed ([[10 blocked]] or unblocked)
![[10 paths 2025-04-24 14.11.59.excalidraw]]

Let there be path 1,2 ,3 etc. these are just combinations of [[10 Causal Structures]], not nodes themselves

If there are no paths between the variables A and B are [[10 (unconditionally) independent|independent]] (imagine 1, 2,3 are just gaps or colliders)

If all paths of dependence are closed or blocked, the 2 variables are [[10 conditional independence|conditionally independent]]

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