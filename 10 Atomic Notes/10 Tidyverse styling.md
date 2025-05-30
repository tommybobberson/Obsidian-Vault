---
Subjects:
  - R
tags:
  - concept
  - academics
aliases:
  - tidyverse style guide
  - R  syntax
status: WIP
created: 2025-05-16 12:37
updated: 2025-05-16 12:37
---
---
## Overview
This documents some commonly confused and niche styling decisions that should be emplyoed when programming according to the tidyverse style guide

### Brackets
When a function spans multiple lines, the closing brackets should be aligned with the start of the function verb it is closing
``
```
mutate(
	one = 1,
	two = 2
) # the bracket aligns with the start of 
```

## Pipes
The base pipe |> should always be preceded by a single space
```
mutate(x = 5) |> # this is correct

mutate(x = 5)|> # this is wrong
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



