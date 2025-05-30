---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - resdiual
status: WIP
---
---
# residuals 
In a fitted linear model, it's the difference between the actual observed values and the predicted value put forth by the model (basically, given the same X or any set of independent variables, what's the difference between the predicted Y and the actual Y, for points where an actual Y datapoint exists)

**Mathematically**: 
$residual_i = Y_i - \hat{Y_i}$
![[10 residuals.png]]

**Characteristics and problems**
- Directional (e.g. -ve or +ve): Thus, it cannot be directly used as a measure of deviation - the [[10 mean squared error|MSE]] must be computed first
- The sum of all residuals = 0, the mean of all residuals = 0 (**in a given linear model**)
## properties of residuals in a linear model
![[10 residuals 1.png]]
**assumptions of the residuals**:
- Normally distributed
- [[10 Homoscedastic]]
- Independent

**assumptions of the variables**:
- there is a linear relationship between the outcome variable and the independent variable
	- characterised by a random scattering of the residuals around the horizontal axis

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