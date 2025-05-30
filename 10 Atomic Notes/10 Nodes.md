---
Subjects:
  - causal inference
tags:
  - concept
  - academics
aliases:
  - node
  - parent
  - child
  - parent node
  - child node
  - ancestor node
  - ancestor
status: WIP
---
---
# Nodes 
Nodes are elements of a graph that are connected by [[10 edges]] 
## R/S between nodes
**parent**: the node from which the arrow (directed edge) starts from
**child**: the node which the arrow from the parent goes into

**parent child relationships are relative to the different nodes we are observing**
	- Y is the parent of L and the child of X etc.
![[10 Nodes 2025-04-23 10.47.23.excalidraw]]
**ancestor**: a special parent node that is the starting node of all nodes connected by a path e.g. X is the ancestor of Y, L and Z

**Configurations**
![[Nodes 2025-05-11 01.33.55.excalidraw]]

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