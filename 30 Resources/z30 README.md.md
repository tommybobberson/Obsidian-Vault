# 30 Resources

## Purpose

Contains notes **about specific sources** (books, papers, courses, etc.). Each note focuses on *one* resource.

## Contents

*   `.md` notes detailing a single source (e.g., `[[Book - Modern Epidemiology (Rothman)]]`).
*   Contains metadata, summaries, links to concepts, and links to attachments.

## Workflow

1.  **Create:** New note per resource using the [T - Resource.md template](../90%20Meta/Templates/T%20-%20Resource.md). Use a descriptive title.
2.  **Add Metadata:** Fill in YAML frontmatter (author, year, tags, URL).
3.  **Summarize & Extract:** Summarize and link key concepts to [10 Atomic Notes](z10%20README.md.md). *(Use specific `[[Concept]]` wikilinks here)*.
4.  **Link Attachment:** Store file in [50 Attachments](../50%20Attachments/README.md) and link it here.
5.  **Add Notes:** Include personal thoughts.

## Using the Template (`T - Resource.md`)

This template helps capture essential information about a source.

*   **YAML Frontmatter:**
    *   `aliases: []`: Add useful shorthands (e.g., `[Rothman Epi]`, `[Pearl 2009]`).
    *   `tags: [resource]`: Base tag. **Add TYPE tags** (e.g., `#book`, `#paper`, `#article`, `#course`, `#video`, `#website`). **Add STATUS tags** (e.g., `#toread`, `#reading`, `#processed`, `#reference`). **Subject tags** (e.g., `#epidemiology`) can be useful here for filtering resources by topic.
    *   `author: [""]`, `year:`, `url:`: Fill in bibliographic details. These are powerful with the Dataview plugin.
    *   `related_concepts: []`: **Manually** add links here to the *key* `[[Atomic Concepts]]` discussed or introduced in this resource (e.g., `["[[Confounding]]", "[[Selection Bias]]"]`). This provides a quick glance at the main topics covered and is useful for Dataview.
*   **`# {{title}}`**: Full title, perhaps Author/Year for papers.
*   **`## Bibliographic Info`**: Pulls info from YAML (requires Dataview/Templater for auto-population, otherwise copy manually) and provides space for full citation if needed.
*   **`## Summary / Abstract`**: Briefly describe what the resource is about.
*   **`## Key Concepts / Takeaways`**: Bullet points summarizing main ideas. **Link heavily** to the corresponding [10 Atomic Notes](z10%20README.md.md) here! (e.g., `- Introduces the idea of [[Potential Outcomes Framework]].`). *(Wikilinks like `[[Potential...]]` are correct)*.
*   **`## Personal Notes / Critique`**: Your thoughts, critiques, etc.
*   **`## Related Resources`**: Link to other notes *within this `30 Resources` folder* (e.g., `[[Another Paper by Author]]`).
*   **Linking the Attachment:** Remember to add a line somewhere linking to the actual file, e.g., `File: [[../50 Attachments/Pearl2009 - Causal Inference Primer.pdf]]`. *(Using `../50 Attachments/...` ensures the link works from within the `30 Resources` folder)*.

**Things to Look Out For:**

*   **Metadata Accuracy:** Fill in YAML fields consistently.
*   **Connecting Concepts:** Use `[[wikilinks]]` in the "Key Concepts / Takeaways" section.
*   **Distinguish Resource Notes vs. Atomic Notes:** Link *to* Atomic Notes, don't duplicate content.
*   **Attachment Link:** Ensure the link to the file in `50 Attachments` is correct (using `../` prefix).

## Template

*   Use the [T - Resource.md template](../90%20Meta/Templates/T%20-%20Resource.md).

## Key Connections

*   Notes are linked *from* [20 MOCs](20%20README.md.md) (as key resources for a topic).
*   Notes are linked *from* [10 Atomic Notes](z10%20README.md.md) (as references/sources for a concept).
*   Notes link *to* [10 Atomic Notes](z10%20README.md.md) (concepts discussed within the resource). *(Use specific `[[Concept]]` wikilinks)*.
*   Notes link *to* files stored in [50 Attachments](../50%20Attachments/README.md).