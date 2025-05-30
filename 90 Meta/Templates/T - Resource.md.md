---
status: 
tags:
  - resource
aliases: 
URL/DOI: 
Subjects: 
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
---
---
# Title
## Chapters

## Related Resources


## Attachment

<%*
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title") 
	text = qcFileName.replace(":", " -")
	titleName = "30" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("30 Resources/"+ titleName);
} else {
	await tp.file.move("30 Resources/" + tp.file.title)
}
-%>