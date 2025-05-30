---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - directional seperation
  - d-seperation
status: WIP
---
---
# d seperation 
A construct to determine whether [[10 Nodes]] are [[conditionally independent]]
- d-seperation means that **every path** between 2 nodes is blocked resulting in [[10 conditional independence]]
![[10 d seperation 2025-04-24 14.25.19.excalidraw]]
imagine A and B as [[10 Nodes]] and N as a set of nodes, P is the [[10 paths|path]] from A to B


**Conditioning N, Path P is blocked ([[10 conditional independence|conditionally independent]]) when**:
1. N contains the central nodes of a [[fork]] or a [[chain]] ([[10 mediator|Mediator]])
	1. You control for the [[10 mediator|Mediator]] or the ancestor in the fork, resulting in conditional independence
2. P contains a collider but the [[10 CI Collider|collider variable]] isn't in N .      
	1. because you're controlling the ancestors of the collider variable (outside of N), thus they are [[10 (unconditionally) independent]]
	2. basically don't control on the collider (or it's [[10 Nodes|child node]]), it's ok to condition on ancestors of colliders 


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