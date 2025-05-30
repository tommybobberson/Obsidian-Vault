---
Subjects:
  - statistics
tags:
  - concept
  - academics
aliases: 
status: revisit add
created: 2025-05-15 01:48
updated: 2025-05-15 01:48
---
---
## Overview 
ANOVA stands for analysis of variance and it tests if the means of 2 (or more groups differs. (*note it can't tell you which of them are different, it can only tell you if they're all the same or not )

$H_0: u_a = u_b = u_c = u_d$
$H_1: u_i \ne u_j$ for some i and j (i. e. not **all** means are equal)

You can think of it as

![[10 ANOVA 2025-05-19 12.53.56.excalidraw]]
By comparing the ratio of the within group variance against the between group variance ([[MSE]], which represents the, we see if the [[MSE]] (within group variance), which also represents the random error not explained by any of the factors, can indeed account for the difference in means of the dependent outcome variable between 2 factors (variance between groups)
![[10 ANOVA.png|600]]
## Types 
**[[One way ANOVA]]**: Used when you have 1 independent variable and with many levels and one dependent variable 

e.g. testing **if there's a difference between** low, medium and high concentrations of chemotherapy on the survival rate of cancer. Here we're testing if the different levels of a single independent variable result in different outcomes (dosage vs survival)

**[[10 Two way ANOVA]]**: Used when have multiple independent variables and one dependent variable. 

Assesses the effect of each independent variable and **the presence of any interaction between them**

e.g. treatment and exercise against cancer survival rates
- you're determining if there's difference in effect between the 2 independent variables. 
- And if they result in a difference in each other when they're both present. Such as when exercise is present, treatment becomes less effective as opposed to when there's no exercise 

<% add different ways to run 2 way ANOVA? %>


## Theory
- Calculates a [[f statistic]] to determine if the difference in the means are due to random noise or actual differences
- This is based off the [[law of total variance ]], that states that the total variance in a source is due to the sum of explained and unexplained variances.
- If there were no difference, the unexplained variance would be the same, but if not it wouldn't be the same 


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



