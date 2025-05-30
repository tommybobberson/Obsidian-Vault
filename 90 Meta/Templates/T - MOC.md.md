---
aliases: 
tags:
  - moc
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
---
---
## Overview 

## Core Concepts / Foundational Ideas


## Chapters 



## Key Resources

## Related MOCs / Areas
<!-- Links to MOCs for related subjects -->


<%*
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title") 
	text = qcFileName.replace(":", " -")
	titleName = "20" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("20 MOCs/"+ titleName);
} else { 
	await tp.file.move("20 MOCs/" + tp.file.title)
}
-%>