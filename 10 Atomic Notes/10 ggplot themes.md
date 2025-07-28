---
Subjects:
  - R
tags:
  - academics
  - resource
aliases: 
status: WIP
created: 2025-06-12 21:13
updated: 2025-06-12 21:13
---
---
## Overview
- this document will just store a bunch of old ggplot themes that i've used with accompanying pictures for future reference

### Black and white theme

![[10 ggplot themes-BnW theme.jpg|500]]
```{r}
theme(
    text = element_text(family = "sans"),
    plot.title = element_text(size = 16, face = "bold", margin = margin(l = 15, b = 10)),
    plot.title.position = "plot",
    axis.title.x = element_text(size = 12),
    axis.title.y = element_text(size = 12),
    legend.position = "bottom",
    legend.text = element_text(lineheight = 0.5),
    legend.margin = margin(t = -10, r = 0, b = 0, l = 0),
    panel.grid.major = element_line(colour = "grey95"),
    panel.grid.minor = element_line(colour = "grey95"),
    panel.background = element_rect(fill = "white"),
    panel.border = element_rect(fill = "NA",colour = "grey90")
  ) +
  
  # sets the background of the legends mapepd to the color aesthetic, to be
  # transparent, replace "color" with any other aesthetic which is mappped
  # to your legend
	
  guides(color = guide_legend(override.aes = list(fill = NA))) +
  
  facet_wrap(vars(parents_highest_education))
```
	



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



