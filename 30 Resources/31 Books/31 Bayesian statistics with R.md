---
status: reference
tags:
  - resource
  - book
aliases: 
URL/DOI: https://statswithr.github.io/book/the-basics-of-bayesian-statistics.html
Subjects:
  - statistics
---
---
# Bayesian statistics with R 

## Summary / Abstract
## Chapter 1 Basics of Bayesian Statistics
### Bayes Rule
The probability of even A conditional on the event B is given by
$P(A|B) = P(A \& B) / P(B)$

Basically you only calculate the probability of the certain event happening within the group you're interested in

### Bayes' rule and diagnostic testing
**In Testing**:
 -**False Positive**: Test returns positive when the truth is negative [[type 1 error]]
 -**False Negative:** Test returns negative when the truth is positive, [[type 2 error]]

- Both have implications, e.g. if you had to screen individuals donating blood for HIV ,
	- Type 1 error: tells people they have HIV when they don't and causes stigma and unecessary stress
	- Type 2 error: accepts a HIV positive person's blood as you mistaken it to be HIV negative and you spread HIV