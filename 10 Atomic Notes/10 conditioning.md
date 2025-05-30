---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - control
  - condition
  - controlling
  - conditioned
status: WIP
---

---
# conditioning 

## Summary/Definition
in research, you control or condition on a variable by holding that variable constant to alter the **flow of dependency** so you can account for the actual effects of other variables to prevent things like confounding

**conditioning** always results in a change in status of the flow of causality, e.g. 
	[[10 CI Chain|Chain]]: conditioning results in the path to be closed 
	[[10 Causal Structures|fork]]: conditioning results in the path to be closed 
	[[collider]]: conditioning opens the path
![[10 Causal relationships 2025-04-23 18.33.56.excalidraw]]
e.g. A is gender, B is construction career or not, C is cancer from abestos
		- males are more likely to be construction workers, thus if we view a to c, it may seem like males are more likely to get cancer from abestos, but that's only because they are more likely to (B) work in construction
		- Controlling for the people who work in construction, i.e. we take the same number of construction and non construction workers from males and females , the rate of cancer form asbestos in males and females is the same


## When to control 
- **Variable is a confounder**: explains variance in both the dependent and predictor variables
- **Variable is a predictor of Outcome**: even if they aren't [[10 confounders|confounder]]s, because they lower the variance of our estimates. As by explaining more of the variance of the dependent variable, they're essentially lowering the portion of the variance which we're trying to fit our variables to. 
## When not to control 
- **Variable is a predictor of the Dependent variable ONLY**: 
	- you increase the variance of the estimator for the dependent variable $\beta$
	- It effectively controls the range of treatments / the dependent variables. And If it doesn't change much, it's hard to estimate it's [[10 Average treatment effect|ATE]]  
    - Mathematically this is because, having a larger range of values of X to estimate the slope, $\beta$ gives you more information to work with 
    - $$
\text{Var}(\hat{\beta}_1) = \frac{\sigma^2}{\sum_{i=1}^n (X_i - \bar{X})^2}
$$
    -  where you're dividing the unexplainable variance in your model (error term) [[mean squared error]] by the variance of your independent variable, X
    - As the variance of X is allowed to increase (for larger ranges of X), the variance of your predictor goes down 

### When it causes [[10 selection bias]]
- **variable is a [[10 mediator]] between the cause and dependent variable**:
	- this has the tendency to cause selection bias as by controlling for this, you're limiting yourself to a subset of the independent variable whose effect you're trying to study
	- 
     -  e. g you control for the stage of schooling which a child is in when you're investigating how age affects a child's vaccine uptake
     - vaccine uptake <- Age - > schooling stage - > vaccine uptake 
     - If You limit yourself to say, primary schoolers, then you might see vaccine uptake increase as age increases, with students getting ready for the move to secondary school 
     - However if you limit yourself to secondary schoolers, you might see vaccine uptake decrease with increasing age as vaccination becomes optional 
     - Overall controlling for mediators can result in a masking of the true causal effect and how they might otherwise differ between different groups 
 - **Variable is a common effect of both the dependent variable (outcome) and treatment:
	 - don't [[10 Conditioning on positives bias| condition on positives]] 
	 - controlling on this results in you choosing only certain  (with certain treatments and outckme of dependent variables) that would have achieved the common effect
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