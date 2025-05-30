# 20 MOCs (Maps of Content)

## Purpose

Provide **structure, context, and navigation** for broader topics, acting as curated tables of contents or dashboards linking concepts and resources.

## Contents

*   `.md` notes serving as high-level guides (e.g., `[[Statistics MOC]]`).
*   Primarily consist of organized lists of `[[Wikilinks]]` pointing to:
    *   [10 Atomic Notes](z10%20README.md.md) (core concepts, methods).
    *   [30 Resources](z30%20README.md.md) (key textbooks, papers, courses).
    *   Other related MOCs.

## Workflow

1.  **Create:** New MOC when a topic feels substantial.
2.  **Structure:** Use headings from the template to organize links logically.
3.  **Link:** Populate by linking *down* to relevant Atomic Notes and Resources. Add brief annotations if helpful.
4.  **Connect:** Link *across* to related MOCs.
5.  **Maintain:** Update as new related notes are added.

## Using the Template (`T - MOC.md`)

This template helps structure your overview of a topic.

*   **YAML Frontmatter:**
    *   `aliases: []`: Useful for shorthand links (e.g., `[Stats MOC]`).
    *   `tags: [moc]`: **Essential tag** to identify this note as a Map of Content. You **can** add relevant **subject tags** here (e.g., `#statistics`, `#epidemiology`) as the MOC *defines* that subject area in your vault. Status tags (`#inprogress`, `#mature`) are also useful.
    *   `created`/`updated`: Auto-timestamps.
*   **`# {{title}} MOC`**: Clear title indicating the subject.
*   **Introductory Sentence:** Briefly state the scope of the MOC.
*   **Headings (`## Core Concepts`, `## Key Methods`, etc.):** These provide structure. Under each heading, create bulleted lists of `[[Wikilinks]]`.
    *   **Links should point primarily to:** Notes in [10 Atomic Notes](z10%20README.md.md). *(Wikilinks to specific concept notes like `[[Concept 1]]` are correct)*.
    *   **`## Key Resources` Section:** Link to relevant notes in [30 Resources](z30%20README.md.md). You can add brief annotations after the link (e.g., `[[Book - Title]] - *Good intro*`). Organize this section (e.g., Textbooks, Papers) if helpful.
    *   **`## Related MOCs` Section:** Link to other MOCs that cover related subjects (e.g., link `[[Statistics MOC]]` from `[[Epidemiology MOC]]`).
*   **Flexibility:** Add, remove, or rename headings as needed for the specific topic. The template is a starting point.

**Things to Look Out For:**

*   **Don't Over-Annotate:** MOCs are primarily lists of links. Keep annotations brief. The details belong in the linked Atomic Notes.
*   **Maintain Focus:** Ensure the links included are relevant to the MOC's topic.
*   **Regular Updates:** As you add new Atomic Notes or Resources, remember to add links to them in the relevant MOC(s). MOCs are living documents.
*   **Balance:** Include links to both foundational concepts and key resources.

## Template

*   Use the [T - MOC.md template](../90%20Meta/Templates/T%20-%20MOC.md).

## Key Connections

*   Provides high-level structure *for* [10 Atomic Notes](z10%20README.md.md) and [30 Resources](z30%20README.md.md).
*   Links *to* notes in `10 Atomic Notes` and `30 Resources`. *(Individual note links via `[[Wikilinks]]` are correct)*.
*   Links *to* other MOCs. *(Individual MOC links via `[[Wikilinks]]` are correct)*.