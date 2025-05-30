---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - treatment
  - intervention
status: WIP
---
---
# treatment 
Refers to some sort of intervention for which we want to know the effect on [[10 Outcomes]]

Represented by T but sometimes by D too

here $T_i$ denotes the treatment staus of the $i$ th individual

can be binary :
T = 1 or T = 0
for cases such as if the medicine was administered vs withheld

can be continuous :
for different doses of a drug administered 

## causal inference
we can't actually give a single individual both treatments (i. e. T = 0 and 1)

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