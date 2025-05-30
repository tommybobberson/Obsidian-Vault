---
Subjects:
  - statistics
  - causal inference
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# Logistic Regression 

## Assumptions
1. The dependent (outcome) variable is binary

2. Observations are independent: 
	- ensure no clustering or repeated measurements (e.g. same age group or location) that result in data being dependent 
	- If clustering exists, you can consider [[mixed effects models]] or [[Generalised  estimating equations]] to account for clustering

3. Adequate sample size
	- 
4. No perfect (Full) or little multi collinearity between independent variables
	- Test by calculating the **Variance Inflation Factor (VIF)** -- assesses how much variance of a regression coefficient is inflated due to linear dependence among predictors
		- To test if variables are collinear, 
	- Remove variables that are collinear when:
		1. Its removal does not significantly impact the model’s interpretability or predictive power.
		2. The variable is not critical to the research question
		3. Other methods to address multicollinearity aren't practical or fail
	
5. Linear relationship between the [[10 logit]] of the response variable and explanatory variables (**not between the explanatory variables themselves unlike in [[10 Linear Regression|linear regression]])
	- For a system where $y = \beta X$, linearity here means that the predictor variable (not just $X$, can also be $X^2$ or $e^X$ etc, that's up to you to define), once defined, is linearly related to the log odds given by $y$.
	  - Can be tested with the [[Box-Tidwell test]]
	
6. Absence of highly influential outliers
	- Can be tested by calculating **Cook's distance** for each observation
	- in the presence of such:
	  1. remove them
	  2. replace them with another value like a mean or median
	  3. keep them and make a note about it when reporting

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