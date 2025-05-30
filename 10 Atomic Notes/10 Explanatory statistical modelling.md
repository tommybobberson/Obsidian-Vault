---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases:
  - explanatory models
  - explanatory modelling
status: WIP
---
---
# Explanatory statistical modelling 

- To test causal hypothesis given a causal theoretical model, to understand the causal mechanisms
- - **the model parameters (indep vars) and the way they're associated with each other and the dependent variable are defined by theory**  

-*where theory is the construct that defines how your independent variables are related and how they are supposed to affect the dependent variable* 
	- e.g. how dd and ss (demand and supply in microecons) are related and in-turn how they affect the price of the good (dependent variable)
	- so if you have a price variation (dependent variable you want to investigate), you can apply the theory of supply and demand, to see if it's supply and demand that has indeed affected your price, or if it's somethin else
	- you are explaining if a theory is the cause of change


- often applied to data for testing causal hypothesis where theoretical constructs (instead of concrete variables) are of interest. -> "does this theory explain my observed variations in my dependent variable"
-
- theory is an immeasurable concept rather than an observable variable that you can measure

let **explaining** == **causal explanation**

**examples**:
[[regression models]]


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