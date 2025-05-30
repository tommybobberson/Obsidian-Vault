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
# Polychoric correlation 
Calculates the correlation between ordinal categorical variables (possible values have a natural order)

Values range from -1 to 1
- -1 = strong -ve correlation
- 1 = strong positive correlation
- 0 = no correlations

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