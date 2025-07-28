---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases:
  - independent
status: WIP
---
---
# independence 
==Being able to assess variables independently of each other is so important because only then can we estimate the true isolated effect, that each variable has on the outcome of interest==

**⫫** : is independent of

## Summary/Definition
- **properties**: independence of variables is a symmetrical relation, if not, they are said to be dependent.
- **Formal definition**: A is independent of B if the ==knowledge that B has occurred gives us no additional information about the probability of A occurring==
$$P(A|B) = P(A)$$
- It then follows that, for every value of A and B that $P(A \cap B) = P(A) P(B)$
- One thing happening doesn't affect the probability of another thing happening


**can be stratified into**:
[[10 conditional independence]]
[[10 (unconditionally) independent|unconditional independence]]

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