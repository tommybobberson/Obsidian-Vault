---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - Dummy variable
status: WIP
created: 2025-05-14 18:45
updated: 2025-05-14 18:45
---
---

## Definition 
A binary (0 or 1) variable that indicates whether something belongs to a group 

## Overview 
Used in [[10 Grouped Regression]] to quantify the effect of subgroups. 

The variable, $X_{group}$
Takes the value of 1 if it (is true that it) belongs to the group and 0 if not

- There will  be n-1 groups such that one of the groups is the default value and all other groups have their effects measured relative to the main group 
## Regression 
Where $\beta_a,\ \beta_b\ and\ \beta_c$  represent the coefficients for group a b and c respectively. in the following grouped regression, 

$Y\ = \beta_0\ +\ \beta_aX_a\ +\ \beta_bX_b\ +\ \beta_cX_c\ + \ \epsilon$ 

When it is in group a, it's not in b and c and so only the effect of a is estimated so on and so forth. 

The fact that they're 0 or 1 helps exclude and distinguish effects of different groups

When all dummy variables=0, we have the default group. All dummy variables and their coefficients are relative to the default group


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



