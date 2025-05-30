---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - collider variable
  - DAG collider
  - collider
status: WIP
---
---
# Collider 

- Unconditioned
	- [[10 (unconditionally) independent|unconditional independence]]: _C_ ⊥ _D_ 
	- closed
- conditioning the collider:
	- dependence, _C_ ⊥⁄ _D_ | _E_ 
	- open
- A path that goes through a collider is **blocked** if you are **NOT** conditioning on the collider or anything that the collider causes.
- The flow of dependency from C to D is [[10 blocked]]
	-  C and D are [[10 (unconditionally) independent]]
	
- The path of dependency can be un[[10 blocked]] by controlling for the collider variable
	- C and D are **dependent** when conditioning on E i.e. [[10 conditional independence]] doesn't hold -



![[Causal relationships 2025-04-24 10.36.14.excalidraw]]
- imagine  C and D (both rivers) flow into E, thus if you [[condition]] on E, the descendant of the ancestors, the flow of C and D must add up (C affects D) and thus they are **dependent** e.g. 
	- E is the probability of getting cancer, C (smoking) and D (asbestos exposure). If there is no D, then there must be C (assuming D and C are the only factors affecting cancer)
- [[10 conditional independence]] doesn't hold either when if, the descendants of E are [[conditioned]] - as you're indirectly constraining the value of E

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