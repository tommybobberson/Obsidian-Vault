---
Subjects:
  - causal inference
tags:
  - concept
  - definition
  - academics
aliases:
  - Outcomes
  - potential outcomes
  - counterfactual outcomes
  - observed outcome
status: WIP
---
---
# Potential Outcomes 
## Summary/Definition
Potential outcomes (aka counterfactuals) and how they differ from observed outcomes [[10 Treatment and Observed outcomes|observed outcomes]]
## Explanation
**Observed outcome** $Y_i$ - think of it as the actual Y for unit $i$ 
**potential outcomes** - we're indecisive so we want to know the outcomes for both treatment optiions: the outcome that would have happened in the case that the other treatment was taken 
	- $Y_{0i}$ - potential outcome for unit $i$ when treatment = 0 aka without the treatment
	- $Y_{1i}$ - potential outcome for unit $i$ when treatment = 1 aka when treatment is given
	-  sometime they are represented in the form $Y_i(treatment)$ where treatment = 0 or 1 
	**both are defined no matter which txt option they receive, we just can't observe the one that didn't happen **
## Example
	- Treatment is the presence of tablets
	- Outcome is the student's test score
- $Y_{0i}$ is the **observed** outcome when a student isn't given a tablet, txt = 0
- $Y_{1i}$ is the **observed** outcome when a student gets a tablet, txt = 1

This can be used to calculate the [[10 individual treatment effect]] for each individual $i$ 

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