---
tags:
  - scribble
status: WIP
created: 2025-04-19 20:34
---
---
# Fleeting Note - 2025-04-19
- General notation
- Association vs causation
- Measures of association and measures of causation
## Idea/Note
### Terms:
	- $Y_i$ = the observed outcome of interest (can be a score, probability any measure) for subject $i$ -- binary, can take on 1 or 0
	- $T_i$ = the given treatment for subject $i$ -- binary, 1 or 0
	-** note that the observed outcome can also take the form of $Y_{xi}$ where $x$ indicates the given treatment (0 or 1)
### Ideas:
To investigate the risk of counterfactual (potential) outcomes when given different treatments, we compare the treatment they received (treated or not treated) with their outcome of interest (happened or didnt happen).

- We can never observe the same individual/subject both with and without the treatment, i.e. We cannot observe $Y_i$ for both $T_i$ = 1 and = 0
- We are trying to make generalisations for the whole **population**, given our experiments on a **sample**

### Measures of causality
1. [[10 individual treatment effect]]: 
	1. $Y_{1i} - Y_{0i}$, the difference in the treatment outcome given treatment = 1 and treatment = 0 for individual $i$
	**Impossible** to actually measure as we can never observe both treatments on one individual

2. Average Treatment Effect :
	1. $ATE$ = $E[Y_1 - Y_0]$, the expected difference in treatment effects between individuals in a sample who have and haven't been treated
	 ** However, 
3. Average Treatment Effect *on the treated*:
	1. 
