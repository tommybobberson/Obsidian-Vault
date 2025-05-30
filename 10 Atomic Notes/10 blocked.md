---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - block
status: WIP
---
---
# blocked 
In causal diagrams and relations, dependency flows through [[10 paths]], to block is to eliminate the flow of dependency from one point to another. 

can be done through [[10 conditioning]]

e.g.
A -> ...... -> B 
if the path is open, dependency flows,
if it is blocked or closed (through [[10 conditioning|10 conditioning]]) there is no flow of dependency from A to B

- blocking is useful when you want to **eliminate** the effect on non-causal [[10 paths]] of interest ([[10 confounders]])

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