---
Subjects:
  - R
tags:
  - academics
  - guide
  - tool
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
### Aesthetic - Group
`aes(group = ....)`, allows you to group certain aesthetics by the provided variable.
e.g., if you want to carry out a weighted regression by the number of observations for each level of influenza vaccination coverage
- `aes(group = influenza_coverage_age, weight = count)`,  will tell ggplot to calculate the weights relative to each level of `influenza_coverage_age`
- where count is the variable representing the number of observations associated with each datapoint
### Aesthetic - Stat
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
	
## Labels
A generic function for all labels can be called with `labs()`. The elements of labs are
```
labs(
	title, # what we're describing
	subtitle, # typically to talk about the context of the study e.g. from 2021
	x,  # x axis label
	y, # y axis label
	caption, # usually for specifics of your data like how it was derived 
	col, # name of the colour aesthetic 
	fill,
	linetype, # legends for all aesthethics can be mapped to have a label
	
)
```
 
 - you can change the name/label of the legend by changing the name of the associated aesthetic e.g. colour
 


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



