---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - GLM
status: WIP
created: 2025-05-08 09:13
updated: 2025-05-08 09:13
---
---
**Components**:
- Intercept, $\beta_0$
- parameters, $\beta_1$
- explanantory variables, $X_1$
- Error, $\epsilon$


**Definition of Linearity**
GLMs are linear with respect to their parameters

- The outcome of interest is linearly related to the [[10 parameters]] ($\beta$), that's to say, the rate of change of Y (outcome variable) with respect to X (explanatory variable) is independent of the value of X, because dy/dx is **only dependent** on the respective parameter $\beta$
- the relationship between the explanatory variables ,X, and Y doesn't necessarily have to be linear, it can be [[10 transformed]] to take the following $X^2, lnX$ etc.

**linear**:
$Y = \beta_0 + \beta_1X_1 + \epsilon$
$Y = \beta_0 + \beta_1lnX + \epsilon$

**non-linear**:
$Y = \beta_0 + e^{\beta_1X_1} + \epsilon$






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



