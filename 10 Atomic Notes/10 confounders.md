---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases:
  - confounding
  - confounder
  - confound
  - confounding bias
  - omitted variable bias
status: WIP
---
---
# confounders 
- The most annoying thing that you want to get rid of
- something that affects both the treatment and outcome of interest (related to both the independent and dependent variable)
- Can result in [[10 Simpson's Paradox]]
- Here L is confounding the relationship between X and Y
![[10 confounders 2025-04-24 15.11.34.excalidraw]]
**FIX**: 
- we want to leave only the direct effect of X -> Y
- [[10 conditioning|control]] all common causes of X and Y (the dependent variable and independent variable), to remove unwanted dependency/backdoor paths

## In Regression
### Why we need to control for omitted variables
- When there is no bias/getting rid of bias:
	omitted variables have no correlation with the dependent variable, and thus it results in no bias, or **all confounding variables are accounted for in the model** (and we wouldn't need to control!)
	
- Omitted variables mask the true r/s between our factors:
	Without accounting for omitted variables (which might be confounders), we can't estimate the effect of the dependent on the independent variables, as:
	
	$regression\ coefficient = \beta hat = \dfrac{Cov(independent_i, dependent_i)}{Var(dependent_i)} = \kappa + \beta'\delta_{omitted variables}$
	
	- where $\kappa$ is the actual effect of the independent on the dependent variable.
	- $\beta'\delta_{omittedvariables}$ is the vector of omitted variables and their regression coefficients
	
	Thus, we can't present the estimated $\beta hat$ as the actual effect, as we are actually presenting an effect by the dependent variable $\kappa$ and more


## Cases  of Confounding
**immeasurable variables**
- You cannot adjust for confounders which are unobservable/immeasurable variables (e.g. Joy)
![[10 confounders 2025-04-24 16.24.50.excalidraw]]
But you can control for **mediators** to the confounder and treatment of interest e.g. smiles per hour. Thus, closing the backdoor path from Joy to Friends, and removing the confounding effect that Joy has on the relationship between one's friends and health

By conditioning on the mediator (smiles) there is [[10 conditional independence]] between Joy and Friends

**surrogate confounders**
In cases where there are immeasurable variables, but there are no [[10 mediator]] variables which you can condition on, you can try to eliminate bias by conditioning on proxies to the confounder, aka surrogate confounders (which lead to the confoudner itself)
![[10 confounders 2025-04-24 16.34.25.excalidraw]]
say we can't or didn't measure smiles per hour, we can get a feel for one's joy by taking reference to things that would have affected it (happy and sad events in their lives) - unable to eliminate [[10 bias]] completely


## Notes
beware of opening up backdoor paths (confounding paths) when you [[10 conditioning|condition]] for [[10 CI Collider|collider]] variables, as collider variables un[[10 blocked|block]] dependencies when conditioned on

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