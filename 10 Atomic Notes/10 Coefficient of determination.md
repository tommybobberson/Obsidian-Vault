---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - R^2
status: WIP
created: 2025-05-21 17:32
updated: 2025-05-21 17:32
---
- statistics---
## Overview
The coefficient of determination, aka $R^2$ value, is a value between 0 and 1, that depicts:
	**the proportion of the variance in the dependent (response) variable that can be explained by the independent (predictor) variable**
- R^2 = 1 indicates that a unit change in the response variable can be **perfectly** explained by our predictor variable
- R^2 = 0 indicates that the predictor variable can't explain our response variable at all

## Caveats
- There is no set value for what is a "good" R^2 value, it depends on your use case your data, and how well you're able to predict the response variable. 
	- In some cases, where stuff is really volatile like stocks even a R^2 of 0.01 would be considered good
	- In other cases such as the social sciences, R^2 values of 0.1 to 0.5 are common

- R^2 Values always increase when you add a variable, no matter how little of the variance of the outcome variable the new variable explains. Thus it isn't always a good measure of goodness of fit as it promotes overfitting. Thus the [[10 adjusted coefficient of determination]] may be preferred

## Calculation
$$R^2 = SSR / SST$$
- where [[10 SSR]] = sums of squares regression (the sum of the squared differences between predicted points on a regression and the mean value of the response variable (dependent variable))
	- SSR is basically the amount of variance (relative to the mean of the response variable) that was explained by the regression line
- where [[10 SST]] = sums of squares Total, the sum of the squared values of the difference between observed data points and mean value of the response variable
	-  SST is the total variance
![[10 SSE 2025-05-21 17.47.22.excalidraw]]

- R^2 = red / orange
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



