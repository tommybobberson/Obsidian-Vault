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
- ==this can be tested by plotting a scatter plot of the predictor variable (input) against the response variable (outcome), and making sure that the r/s is indeed roughly linear==, else, you must [[10 transformed|transform]] either the predictor or the outcome to make sure that they're linear with each other. (though usually it's the predictor variable as the outcome variable is linearly related with many other vars too)

**General Form**: 
- Takes the same form as in [[20 Regression MOC]]

**conditions**:
- all parameters ($\beta$) enter the model linearly, with or without [[10 transformed|transformation]] of the data


**Challenges**:
- [[10 grouped data]]

## Regression Terms
### Predictors
 **Magnitude**: 
 - of the coefficient of each respective variable $i$, $\beta_i$, represents the unit change of the dependent variable with each unit change in each variable i
 **$R^2$:
 - ** of each coefficient, represents the **proportion of variance seen the dependent variable, Y** that each variable explains
![[10 mean squared error 1]]
**p-value**:
- **for a categorical predictor**: if the predictor variable results in a statistically significant change in the response variable
- **for a continuous predictor:** if the average change in the response variable / unit of the predictor is [[statistically significant]] from 0

## Regression Theory
For all regressions, different ways of fitting the regression line can be employed. However, the most commonly used for linear regression are:
- [[10 OLS]] is usually employed where you're solving a equation for the values of a **predictor(s), $\beta$, that minimize(s) the [[10 mean squared error]]** between your actual value, and predicted value.
- [[10 Weighted Regression|Weighted least squares]]
- [[Partial Least Squares]]

## Things that hold true for linear regression
1. **the sum of all the variables and their slopes (effects) gives you your total effect**: 
- Due to the [[38 Multiple linear model assumptions|linear model assumptions]], you're just quantifying the proportion of each result that is explained by each variable in the model.
	- the total effect of X on Y is equal to the sum of the direct and indirect effects of X

2.  **The indirect effect of X on Y through M is the product of each of the indirect effects through that respective causal path (i.e. X on M and the effect of M on Y**)![[40 Attachments/10 Linear Regression]]
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