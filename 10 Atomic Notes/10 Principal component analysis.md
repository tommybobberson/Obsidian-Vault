---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
aliases:
  - multivariate analysis
status: WIP
---
---
# Principal component analysis 

re expressing chosen factors from a dataset (into ordered principal components) that give you the most information whilst minimizing the number of variables and thus uncertainty/messiness

_"A method to re-express multivariate data, such that the first few expressions account for as much of the available information as possible"_

PCA aims to reduce the number of variables by reassigning your current variables into *principal components*, which are ranked, in terms of the amount of variance of a dataset they explain

**Assumptions**: 
	each property is uncorrelated with all others to eliminate [[multicollinearity]] when using the results in analysing dependence
	

**uses**:
best used for [[10 predictive statistical modelling|predictive modelling]]

**methods**: 
- [[dimension reduction]]:
	- takes linear combinations of original variables to form new "principal components" - which are **ordered** based on the amount of the [[10 variance]] they explain
- identifying association between original variables and principal components

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