---
Subjects: 
tags: []
aliases: 
status: WIP
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>
---
---
<%* 
if (tp.file.title.toLowerCase() === "untitled") {
	let qcFileName = await tp.system.prompt("Note Title")
	text = qcFileName.replace(":", " -").trim()
	titleName = "10" + " " + text  
	await tp.file.rename(titleName)
	await tp.file.move("10 Atomic Notes/"+ titleName);
} else {
	await tp.file.move("10 Atomic Notes/" + "10" + " " + tp.file.title)
}
-%>



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



