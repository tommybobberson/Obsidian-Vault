---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - COP bias
status: WIP
created: 2025-05-24 02:12
updated: 2025-05-24 02:12
---
---
## Overview 

It occurs when you condition on an outcome that is itself a consequence of the treatment or, a shared cause of the treatment and another variable that affects treatment 
![[10 Conditioning on positives bias.jpg]]

- Essentially by fixing the comparison of people who achieved a positive (or negative) outcome, you're limiting yourself to a subset of individuals who were more likely to have achieved the result, regardless of the treatment.

- This applies even if the initial treatment was randomly assigned, with the 2 groups having different inherent characteristics 
## Example 
Imagine treatment T makes it easier for people with very severe underlying conditions to achieve a positive outcome (Y>0).
 * Control group: Only the inherently healthiest people manage to achieve Y>0.
 * Treatment group: The treatment helps both the healthy and some of the very sick people to achieve Y>0.
If you then compare E[Y | Y > 0, T=1] with E[Y | Y > 0, T=0], you are comparing the outcome for a group that includes some very sick individuals (in the treated group) with a group of inherently healthier individuals (in the control group). The comparison is no longer "apples to apples" because the composition of the "positive outcome" group has been selected differently due to the treatment, even though the initial treatment assignment was random. 

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



