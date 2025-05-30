---
aliases:
  - directed acyclic graphs
  - DAG
tags:
  - concept
  - academics
Subjects:
  - causal inference
status: WIP
---
---
# Directed Acyclic Graphs (DAG)
## Summary/Definition
A graph that illustrates the dependencies and links between different variables, allowing us to identify causal relationships of importance, DAGs enable us to diagnose which [[10 bias]] we are working with and the tools we need to correct them

**application**:
DAGs allow us to study the causal relationships we want to study by [[10 blocked|block]]ing non-causal [[10 paths]] (backdoor paths) and keeping the causal paths of interest open


**By definition, it has the following characteristics**:
	- **directed**: every edge has a direction
	- **acyclic**: no directed cycles i.e. one variable cannot point back to itself 
	- ([[10 Nodes|ancestor]])s cannot be their own descendants
![[Causal Path]]

**elements**:
	- **Arrow**: represents a *possibly non-zero* causal effect
		- that is to say that an exclusion of an arrow is a bolder claim than the inclusion of one because with an arrow you are only saying that there *may* be a relationship
		- ![[DAGs 2025-04-23 10.42.10.excalidraw]]
		- X -> Y means X may or may not affect Y; the absence of an arrow from x to y means there is **no** causal r/s
	- **[[10 Nodes]]**: elements/variables linked by arrows
	
**limitations:**
	- represents the causal direction but doesn't contain information about its' **functional form** i.e. how the 2 variables are related

**possible relationships** :
	- [[10 common cause]]

**configurations**:
	- [[10 CI Collider]]
	- [[10 CI Fork]]
	- [[10 Causal Structures]]
	

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