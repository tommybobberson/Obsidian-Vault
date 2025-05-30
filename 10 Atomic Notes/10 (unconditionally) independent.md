---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - unconditional independence
  - independent
status: WIP
created: '<% tp.date.now("created: <% tp.date.now("YYYY-MM-DD HH:mm") %>updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>YYYY-MM-DD HH:mm") %>'
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
---
---
# (unconditionally) independent 

- What we usually mean by [[10 independence]] 
- the value of 2 variables are not dependent on the value of each other
- **doesn't hold** sometimes when you end up [[10 conditioning]] on variables like [[collider]]s 

**mathematically**:
	P(A n B) = P(A) P(B)

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