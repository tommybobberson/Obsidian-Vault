---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases: 
status: WIP
---
---
# covariance 
 - A measure of the direction (**but not strength**) of the relationship between 2 variables, i.e if they both increase together, or if one decreases while the other increases
 - **units**: depend on the variables being measured
 - **range**: $- \infty to \infty$
 
![[Pasted image 20250430120214.png]]

## Properties of Covariance
1. **Covariance is commutative**: $cov(x,y) = cov(y,x)$ for any random variables $x,y$

## methods for measuring covariance
**categorical-continuous**: density plots against the continuous variable (stratified by the categorical variable) e.g. a box plot showing how each category (type of house) fares with the continuous variable (price of house) or the densities of price (price of house) against type of house
**categorical-categorical**: count the number of observations for each combination of 2 variables, covariation presents as a strong relationship between certain x and y variables
**numerical-numerical**:
- scatter plots (x against y)
- or for larger datasets create bins of one continuous variable and create box plots for each bin (x) against y

## limitations:
- depends on the units and thus makes it hard to interpret if the variables measured are of different units
- only works for straight line r/ss
- doesn't show how strong the relationship is

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