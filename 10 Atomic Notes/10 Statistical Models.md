---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
aliases:
  - statistical modelling
  - models
  - modelling
status: WIP
---
---
# Statistical Models 

Used differently to either explain [[10 causation]] or to predict future outcomes. 

A __common misconception__ is that explanatory power (explaining causation) also hold high predictive power. Thus explanatory and predictive models are often conflated

However, there are different types of models that are built for each:
[[10 Explanatory statistical modelling]]
	- common in economics, psychology and education to explain the effect something has on their outcome of interest
	- testing if theory A explains the variation in a dependent variable of interest, B
[[10 predictive statistical modelling]]:
	- bioinformatics or linguistics, to predict things
	- How does our dependent variable B, change with our inputs
[[10 descriptive statistical modelling]]:
	- to summarise and represent data in a compact manner
	- there is a less formal emphasis on / no emphasis on [[10 causation]]
	- Also focuses on describing variables that can be and are actually measured 
	- What is the [[10 association]] between our independent variables and dependent variable, B


## Methods for modelling:
[[20 Regression MOC]]




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