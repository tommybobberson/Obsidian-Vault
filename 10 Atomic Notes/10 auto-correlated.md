---
Subjects:
  - statistics
tags:
  - academics
  - concept
aliases: 
status: WIP
created: 2025-06-09 17:04
updated: 2025-06-09 17:04
---
---
## Summary

## Overview
`Where each observation is dependent on other observations (e.g. maybe previous point of time)`

**issues**:
- standard errors become unreliable

**how to detect**:
- [[Durbin-Watson test]]: detects first order autocorrelation


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



