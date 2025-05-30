---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases:
  - constant variance
  - homoscedasticity
  - heteroscedasticity
status: WIP
---
---
# Homoscedastic 

- it refers to when the [[10 variance]] of a variable remains constant for all values of that variable
- its opposite is heteroscedasticity, where the variance of a variable doesn't stay constant for all values of that variable
![[Pasted image 20250511032606.png]]
## causes of non-homoscedasticity (heteroscedasticity)
- [[10 grouped data]]: data from smaller samples will have a larger variance than data from larger samples though each sample contributes to a data-point (say mean value) - this shows up as a non uniform distribution of the data points
- e.g. points to the right have less variance as compared to the points on the left, thus there is heteroscedasticity in the data comparing average score to the number of students in a school
	![[Pasted image 20250511032429.png]]
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