---
Subjects:
  - causal inference
tags:
  - concept
  - definition
  - academics
aliases:
  - treatment effect
  - indiv treatment effect
status: WIP
---
---
# individual treatment effect
## Summary/Definition
$Y_{1i} - Y_{0i}$ : the individual treatment effect is the difference in outcomes **for a specific individual** $i$ when treatment is given and is not given - and if you know this then you know the effect of the treatment

- this is **impossible to observe**, as we can never observe both [[10 Outcomes]] for a specific individual 
- this ensures there's no [[10 bias]] affecting the difference in outcomes 

To study the effect of treatment on outcomes, we can then use the [[10 Average treatment effect]]

## Explanation

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