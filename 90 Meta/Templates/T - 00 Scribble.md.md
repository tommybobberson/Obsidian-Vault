---
tags:
  - scribble
  - academics
status: unread/notes taken/processed
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
source:
---
---
# Scribble - {{date:YYYY-MM-DD}}



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