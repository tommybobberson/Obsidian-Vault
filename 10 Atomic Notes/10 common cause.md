---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - DAG relationships
  - common cause
status: WIP
---
---
# common cause 

## Summary/Definition
![[10 common cause 2025-04-23 18.25.25.excalidraw]]
## Explanation
L is an [[10 Nodes|ancestor node]] of both X and Y

When Y <- L -> X -> Y, L is a [[confounder]]

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