---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - Sum of squared error
  - Unexplained Error
status: WIP
created: 2025-05-19 12:15
updated: 2025-05-19 12:15
---

## Overview
The sum of squared errors refers to the variance between the observed and predicted values

## Calculation
It is given by the sum of squared residuals in a regression. i.e. (difference of the value of the true value of a point - the predicted value of a point) ^2

$SSE = \sum_{i=1}^{n} (Y_i - \hat{Y}_i)^2$

![[10 SSE 2025-05-21 17.47.22.excalidraw]]
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



