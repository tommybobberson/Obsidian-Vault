---
tags:
  - scribble
status: WIP
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
---
---
# Scribble - {{date:YYYY-MM-DD}}

<!-- Quickly jot down thoughts, ideas, reminders, or raw notes here. -->
<!-- Aim to process these notes regularly. -->

## Idea/Note


<%*
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title") 
	text = qcFileName.replace(":", " -")
	titleName = "00" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("00 Scribbles/"+ titleName);
} else {
	await tp.file.move("00 Scribbles/" + tp.file.title)
}
-%>