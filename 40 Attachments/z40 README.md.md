# 40 Attachments

## Purpose

Stores all **non-Markdown files** (attachments) like PDFs and images, linked *from* your `.md` notes (primarily Resource notes).

## Contents

*   PDF files, image files, other relevant non-Markdown assets.


## How your vault handles different files
1. **Excalidraw**: Naming of these files are handled by excalidraw itself, which gives it the name **"{NOTE NAME} dd-mm-yy.excalidraw"**, where {NOTE NAME} refers to the name of the note in which the excalidraw drawing was first embedded. If you're reuse the same drawing in another note, it will just link it to the original note's drawing so take note. **This is not being handled by the custom attachment location plugin because it's quite glitchy so it's just saving to `40 Attachments` for now**.

2. **Custom Attachment Location**: Handles all non excalidraw.md files right now. What it should do is, create a note in a folder under `40 Attachments` that corresponds to the folder you were working in. And it's named according to the note which you were working in.


	An example is attached below
	![[z40 README.md 30-05-25.excalidraw]]
	Thus say i'm working on [[10 Two way ANOVA]], which is under `10 Atomic Notes`, pasting an image in the note results in an attachment that will be `40 Attachments/10 Atomic Notes/10 Two way ANOVA.png`

	**note for books and resources**: when you want to import a book or any resource into obsidian, due to the nature of the file handling, create a note for that resource under `30 Resources` first, and then drag the pdf into the note. This way it's handled properly by the custom attachments plugin
## Workflow & Best Practices

2.  **Configure Obsidian:** Ensure `Settings` -> `Files & Links` -> `Attachment folder path` is set correctly to `40 Attachments` (or your chosen name).
3.  **Add Files via Linking:** The best way is to **drag-and-drop** a file onto the `.md` note it relates to (usually a note in [30 Resources](z30%20README.md.md)). Obsidian will copy the file here and create the link automatically.
4.  **Avoid Direct Edits Here (Usually):** Manage these files *through* Obsidian.

## Template

*   N/A (Contains actual files, not template-based Markdown notes).

## Key Connections

*   Files here are linked *from* `.md` notes elsewhere (mainly from notes in [30 Resources](z30%20README.md.md)).
*   Centralizes assets, keeping other folders clean.