---
Subjects:
  - statistics
tags:
  - academics
aliases:
  - smoothing plot
status: WIP
created: 2025-06-22 14:22
updated: 2025-06-22 14:22
---
---
## Overview
- A form of localised regression where we calculate an estimator, Y_hat, for each pint we have, $Y_i, based on a smaller set of data
- 

### Steps
Esentiallly, fitting a curve with the loess method is done by:
1. splitting the data into many sets of points (as a proportion of the total number of points) - we will cycle through each "window" for all the points
2. At **each data point**, fit an estimated line using some form of least squares (mostly [[10 Weighted Regression|Weighted least squares]])
3. We then walk through each  point in the set, defining one as a focal point one at a time, and apply [[10 Weighted Regression|Weighted least squares]], attributing more weight to points that are closer to the focal point. -- **calculating a line of best fit per window, and taking the point on the line that has the same X value, Y hat, as the focal point, $Y_i$**
	![[10 loess 22-06-25.excalidraw]]
4. We then calculate the distance between each of our estimated points, Yhat, and $Y_i$. 
5. Repeat steps 2-4, using $\delta Y$ as an additional weight together with the weights on the x axis, per window and focal point -- this accounts for extreme outliers on the y Axis
	![[10 loess-loess, Y weights.jpg]]
6. you have now obtained you "new-new" points and the curve formed should be much smoother
7. repeat as many times until you get a nice smooth curve to fit the data
## additional considerations
### Fitting Lines/parabolas within each window
- **within each window**, we can fit a line or parabola to the data
	![[10 loess-fit parabola vs line.jpg]]
### Fitting Lines/parabolas In R
- `Lowess()`: only fits a line 
- `Loess()`: can fit a line or parabola(default)  + can draw [[10 Confidence Intervals]]
### Number of points
- you can vary the number of points fit per window, usually as a proportion of the total number of points
- the smaller the proportion, the more fine grained the curve will be

### choices for weight funtions
- they are arbitrary and there is no reason why they're chosen

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



