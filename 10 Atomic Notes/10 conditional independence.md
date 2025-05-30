---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - conditionally independent
status: WIP
---
---
# conditional independence 
- 2 variables are independent when another common variable is known (conditioned for)
	- Can be determined by the [[10 d seperation]] rule
- A and C are independent when B is [[conditioned]] for
- A and C are dependent when B is not [[conditioned]] 
![[10 Causal relationships 2025-04-23 18.33.56.excalidraw]]
**mathematically**:
	$P(A \cap C | B) = P (A | B) P (C | B)$ 
	$P(A | C \cap B) = P(A|B)$
	- basically, when B is given, the value of the variables of interest (A and C) are independent of each other

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