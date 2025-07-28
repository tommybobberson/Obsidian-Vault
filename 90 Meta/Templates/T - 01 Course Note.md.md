---
tags:
  - "#course"
  - "#academics"
course: 
status: unread/notes taken/processed
created: 
updated:
---
# Summary

# Concepts

# Attachment

<%* 
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title")
	text = qcFileName.replace(":", " -").trim()
	titleName = "01" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("00 Scribbles/"+ titleName);
} else {
	await tp.file.move("00 Scribbles/" + "01" + " " + tp.file.title)
}
-%>