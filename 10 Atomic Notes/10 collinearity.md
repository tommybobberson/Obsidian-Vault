---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - multicollinearity
status: WIP
---
---
# collinearity 
- when predictor variables are perfectly (or very much) correlated with each other
- Measure of [[10 correlation]],$R^2$, is close to 1, 
	- Thus they "tell the same story"
	- Having multiple such variables makes it difficult for the model to identify which variable/how each variable is contributing to the dependent variable

**actions** 
- If it is a [[10 confounders|confound]]ing variable, it should be included so it can be controlled for. ELSE
- Should be accounted for and excess variables that are collinear, removed, for multiple linear regression 

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