---
Subjects:
  - R
tags:
  - concept
  - academics
aliases:
  - ggplot
status: WIP
created: 2025-05-08 14:15
updated: 2025-05-08 14:15
---
---
## Summary 
A plotting software

## Elements of a ggplot
A ggplot can be built 4 things
```{r}
ggplot(you can put your mappings here or in the individual layers) +
geom_XXXX() +
labels() +
theme()
```
- ggplot(): the base layer plotting object
- [[ggplot geom|geom_xxxx]](): a graph or thing that you want to plot as a layer
- [[ggplot labels|labels]](): includes titles and everything else that you can add
- [[ggplot theme|theme]](): allows you to format the elements of your plot (labels and geoms), or use imported themes
## Elements of a ggplot
### Stat
The value that the particular geom displays, can be mapped to aes(x, y, stat)
- must be referred to by .. ..
	- e.g. `geom_bar(aes(y = ..prop..))`
	- here `aes(y = prop)` would just refer to some variable in our dataset (even if there isn't one)
**stats**:
The stats that can be passed depend on the graph being plotted
	 `identity`: take the value of the variable as is
- `geom_bar`
	- `prop`: bars as proportions
- `geom_density`
	- `density`: default density
	- `scaled`: proportional density (relative to the maximum density along the graph)
	- `count`: number of oservations * density
	



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



