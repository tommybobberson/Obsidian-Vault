---
Subjects:
  - statistics
tags:
  - academics
aliases: 
status: WIP
created: 2025-06-07 22:38
updated: 2025-06-07 22:38
---
---
## Overview

If A and B are events with P(B) > 0, the probability of A given B is defined as
$$P(A|B) = \frac{P(A\cap B)} {P(B)}$$

- essentially, when you're looking at the probability of A, when B is your frame of reference, instead of your whole sample space.
- This is achieved by [[normalising]] the probability of A wrt B
-  ![[10 intersection 07-06-25.excalidraw]]


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



