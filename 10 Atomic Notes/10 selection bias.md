---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# selection bias 
- basically, inadvertently,choosing from a group that has predefined characteristics or choosing a group taht has predefined characteristics. Thus resulting in dependencies which mask the real causal relationship you're trying to study 
- occurs when we condition on a [[10 CI Collider|collider]] variable between our independent variable and our dependent variable
- in the context of the river flow, there is now a dependency between the indep variable and the dependent variable as their total "flow" must add up to the "flow" of the collider variable

## Mathematically
$$E[Y_0|T=1] \ne E[Y_0|T=0] $$
The expectation of the outcome (dependent variable, Y) when given no treatment $Y_0$ was different between the group which actually received the treatment and the group that didn't receive the treatment. 
## example
![[selection bias 2025-04-30 11.39.00.excalidraw]]
- Where the green arrow is the causal r/s of interest. When we control for life expectancy, only certain combinations of income and vax uptake can exist to give our selected value of life expectancy
- Thus, a path of dependency has been opened up between vax uptake and income.
	given the same life expectancy, these are the possible combination of factors:
		- higher income (better healthcare, living environment etc) + lower vax uptake (less resistance against disease)
		- lower income (worse living conditions, social determinants of health) + higher vax uptake (more resistance against illness)
	- Thus, it would seem that income is inversely related with vaccine uptake but this isn't the true causal relationship

## Controlling
- never [[condition]] on variables which might cause selection bias 
- here it's the red variables 
	- mediator between the treatment (T) and outcome (Y) 
	- common effect of the treatment and outcome - - this results in the 
![[Pasted image 20250524020914.jpg]]


## Types of selection bias
- [[10 Conditioning on positives bias]]
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