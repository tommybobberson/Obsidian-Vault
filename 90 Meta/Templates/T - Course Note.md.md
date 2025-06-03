---
tags:
  - "#course"
  - "#academics"
course: 
status: unread/noted/processed
created: 
updated:
---
<%* 
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title")
	text = qcFileName.replace(":", " -").trim()
	titleName = "32" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("30 Resources/32 Course Notes/"+ titleName);
} else {
	await tp.file.move("30 Resources/32 Course Notes/" + "32" + " " + tp.file.title)
}
-%>