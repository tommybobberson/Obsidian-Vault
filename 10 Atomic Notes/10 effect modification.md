---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# effect modification 
## Overview

**The case when the nature of the relationship (size/direction) between variable A and B are modified by the presence of a third variable C.**

e.g.
when the presence of cancer is an effect modifier,
In its absence, weight increases with age
In its presence, weight decreases with age

![[10 effect modification 10-06-25.excalidraw]]

- Importantly, effect modification can be multi dimensional
- effect modification is, mathematically, **==commutative==**. in a regression equation where it shows up as $Weight = \beta_ 0 + \beta_1Age + \beta_2Cancer +\beta_3(Cancer)(Age) + \epsilon$, 
	- it makes sense that the presence of cancer affects the relationship between age and weight, but the converse is also true, that different ages will result in different weights when holding the presence of cancer constant
	- However, __we are usually only interested in studying the effect in one direction, which may make more practical sense__
### How it shows up
- 

### Special cases: Effect modification by proxy
- ![[10 effect modification-Effect modification by proxy|1294]]
 - where Q can indirectly modify the relationship between A and Y
 - note that here graphs **A** and **B** are representing the same thing, just that one is an [[IDAG]]
## Causality
**Requirements for effect modification**:
- A variable must directly influence the outcome of interest for it to modify the effect between another variable and the outcome of interest, In DAG terms:
  ![[10 effect modification 05-06-25.excalidraw]]
		"Once you have drawn your DAG, you already assume that any variables pointing to the same outcome can modify the effect of the others pointing to the same outcome. It is a modeling assumption, separate from the DAG, which presumes the lack of an interaction."


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