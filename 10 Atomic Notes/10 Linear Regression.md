---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - linear regression
status: WIP
---
---
# Linear Regression 
To determine the relationship between a continuous ([[10 simple regression|Simple]]) / many continuous variables and the dependent variables [[10 multiple regression]]

**Linear**: refers to how the outcome variable is a continuous variable, linearly related to the independent variables

**General Form**: 
- Takes the same form as in [[20 Regression MOC]]

**conditions**:
- all parameters ($\beta$) enter the model linearly, with or without [[10 transformed|transformation]] of the data

**Assumptions, for multiple linear regression**
- no [[10 collinearity]] except in the case of confounding
- there is a linear relationship between the dependent and independent variable
- The residual values are:
	- normally distribued (plot histogram of residuals)
	- [[10 Homoscedastic]] (have a constant variance for all values of the variable) 
	- Independent
- There is the need to account for, [[10 effect modification]]

**Challenges**:
- [[10 grouped data]]

## Regression Theory
For linear regression, [[10 mean squared error|OLS]] is usually employed where you're solving a equation for the values of a **predictor(s), $\beta$, that minimize(s) the [[10 mean squared error]]** between your actual value, and predicted value.



## Things that hold true for linear regression
1. **the sum of all the variables and their slopes (effects) gives you your total effect**: 
- Due to the [[30 Multiple linear model assumptions|linear model assumptions]], you're just quantifying the proportion of each result that is explained by each variable in the model.
	- the total effect of X on Y is equal to the sum of the direct and indirect effects of X

2.  **The indirect effect of X on Y through M is the product of each of the indirect effects through that respective causal path (i.e. X on M and the effect of M on Y**)![[Regression 2025-05-11 02.51.26.excalidraw]]
	- This doesn't hold for [[10 Logistic Regression]] as we're not dealing with slopes (which are directly additive) but with [[10 logit|log odds]] (or the [[odds ratio]] instead), thus when we have $OR_{XM} * OR_{MY}$we aren't getting the sum of the odds ratio anymore, but rather some weird number, the ORs have to be summed instead.

3. The [[10 confounders|omitted variable bias]] or bias from [[10 confounders]] is equal to the product of X on M and X on Y can be calculated from the following mantra:
	"Basically when we don't control for the confounder, the effect of our dependent variable = true value of independent variable on dependent variable + effect of confounder on dependent variable * effect of confounder on independent variable"
	
	"Short equals long 
	plus the effect of omitted 
	times the regression of omitted on included"
	
	$β1=\beta_2 + \gamma \times \delta$

	for the following set of equations:
	- Short regression model:
	    $Y_i = \alpha_1 + \beta_1 X_i + u_i$​
	- Long regression model:
	     $Y_i = \alpha_2 + \beta_2 X_i + \gamma Z_i + \epsilon_i$    
	     
	    where $Z_i$ is the omitted variable in the short regression.
	    **notice how the coefficient of the dependent variable $X_i$ has changed
	    
	- $\beta_1$​ is the coefficient in the short regression (omitting the relevant variable).
	- $\beta_2​$ is the coefficient in the long regression (including the relevant variable).
	- $\gamma$ is the effect of the omitted variable Z on the dependent variable Y.
	- $\delta$ is the regression coefficient of the omitted variable Z on X, given by:
		    $δ = \frac{\text{Cov}(Z, X)}{\text{Var}(X)}$ 
		    **basically, it's quantifying the effect that our omitted variable Z changes with each X
	
	The OVB formula is specific to linear regression and does not hold in this form for nonlinear models.
	    


    


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