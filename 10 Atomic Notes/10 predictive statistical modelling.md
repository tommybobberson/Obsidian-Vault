---
Subjects:
  - causal inference
  - statistics
tags:
  - concept
  - academics
aliases:
  - predictive modelling
  - predictive models
status: WIP
---
---
# predictive statistical modelling 
- designed to take an input of **variables** and predict and output, instead of testing for a causal hypothesis (if there is causation or not)
- Not heavily based in theoretical constructs or interested in examining the association of theoretical constructs as compared to [[10 Explanatory statistical modelling|explanatory  models]]
- The goal is to build a model that can most accurately forecast the outcome for new data, regardless of whether the relationships are truly causal or just correlational (though understanding the causal relationships definitely helps)
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