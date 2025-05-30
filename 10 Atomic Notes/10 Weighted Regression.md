---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - Weighted Regression
  - Weighted least squares
status: WIP
created: 2025-05-11 03:28
updated: 2025-05-11 03:28
---
---
## Overview
$Weight = 1 / variance = 1 / \sigma^2$

## Use cases
- To handle [[10 Homoscedastic|heteroscedasticity]]
- account for sample misrepresentation
- account for duplicate observations


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



