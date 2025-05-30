---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - Chain
  - causal diagram chain
  - DAG chain
status: WIP
---
---
# Chain 
- only one way arrows
- typically, without conditioning: A ⫫/ C
- [[10 conditional independence]]: _A_ ⊥ _C_ | _B_
	-![[Causal relationships 2025-04-23 18.33.56.excalidraw]]
	- the flow of dependency from A to C is not [[10 blocked]]
	- Flow from A to C can be blocked by [[10 conditioning]] B, only when C's only parent is B 
	- B is a [[10 mediator]] 
	- A and C are [[10 conditional independence]]
	- e.g. A is gender, B is construction career or not, C is cancer from abestos
		- males are more likely to be construction workers, thus if we view a to c, it may seem like males are more likely to get cancer from abestos, but that's only because they are more likely to (B) work in construction
		- Controlling for the people who work in construction, i.e. we take the same number of construction and non construction workers from males and females , the rate of cancer form asbestos in males and females is the same
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