---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - collider
  - chain
  - fork
  - DAG structures
  - causal structures
status: WIP
---
---
# Causal Structures 
## Summary/Definition
The relationships in causality can be classed differently based on the presence and direction of arrows
**[[10 CI Chain]]**: 
	A -> B -> C
	- results in [[10 mediator|Mediator]]s
	- _A_ ⊥ _C_ | _B_
	- open path
**[[10 CI Fork]]**:
	 D <- B -> C
	 - _C_ ⊥ _D_ | _B_
	 - open path
**[[10 CI Collider]]**:
	 D -> E <- C
	 - _C_ ⊥ _D_ and _C_ ⊥⁄ _D_ | _E_ 
	- closed path 
	- A path that goes through a collider is **blocked** if you are **NOT** conditioning on the collider or anything that the collider causes.

**Illustration**

![[10 Causal Structures.png]]
- Open arrows: [[10 independence|independent]]
- tipped arrows: dependence
- Grey Indicates [[10 conditioning]]

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