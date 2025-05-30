---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases: 
status: WIP
created: 2025-05-09 11:05
updated: 2025-05-09 11:05
---
---
## Definition
Simpson's paradox is when a trend (or lack thereof) in aggregated data appears or reverses after being divided into subgroups
![[Pasted image 20250509113323.png]]
## Causes
- [[10 confounders|confounding]], though not always?
- differences in collected data (refer to example)![[10 Simpson's Paradox 2025-05-11 01.26.38.excalidraw]]
## Example
An example of simpson's paradox due to confounding is us investigating the effect of a cancer drug on the survival of a hospital's population

Overall, it might seem like the drug actually results in more death. 

However, once we stratify the data by individual's sex, we realise that:
- for age <50, survival rates **increase**
- for age > 50, survival rates **decrease**

As such, we can say that age here is a confounder.

**However, what if it turns out that in our not so perfectly randomised trial, we somehow managed to give mostly the people who were younger, the drug. in this case where one's age isn't causally related to the likelihood of them getting the drug, is this still a case of simpson's paradox? (or is this not applicable because we aren't specifically looking at the subgroups within each of these age categories that received treatment)
![[10 Simpson's Paradox 2025-05-09 11.29.30.excalidraw]]

in 

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



