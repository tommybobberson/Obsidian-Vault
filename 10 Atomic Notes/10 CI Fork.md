---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - Fork
  - Forks
status: WIP
---
---
# Fork 
- A type of relationship between variables in causal diagrams
- The flow of dependency is un[[10 blocked]] between C and D
- [[10 conditional independence]] achieved when controlling for B: _C_ ⊥ _D_ | _B_
	- as you close the open path between C and D
- two arrows stemming from the middle node
	- given the common ancestor (B), the branches of a fork (C & D) are independent i.e. [[10 conditioning]] for B, C and D are not [[associated]]
	- 
	![[Causal relationships 2025-04-23 18.44.58.excalidraw]]

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