---
Subjects:
  - statistics
tags:
  - academics
aliases:
  - intersection of events
status: WIP
created: 2025-06-07 22:24
updated: 2025-06-07 22:24
---
---

## Overview

### Probability of the intersection of 2 events
$$P(A \cap B) = P(A)P(B),\ when\ A\ and\ B\ are\ independent$$
$$P(A\cap B) = P(B)P(A|B) = P(A)P(B|A)$$

- This is a rearrangement of the definition of [[10 conditional probabilities]]
- ![[10 intersection 07-06-25.excalidraw]]-==note that P(A|B) is not always equals to P(B|A)== and they are non-[[commutative]]

### Probability of the intersection of n events
- For events $A_1, ..., A_n$ with $P(A_1, ..., A_n) > 0$
- 
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



