---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# Cramer's V 
Calculates the correlation between nominal -- variables with no natural ordering -- categorical variables

Ranges from 0 to 1
- 0 = no association between the varaibles
- 1 = strong association between the variables

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