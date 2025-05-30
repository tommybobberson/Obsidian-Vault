# 10 Atomic Notes

## Purpose

This is the **core knowledge base**. Each note covers **one specific concept, definition, method, etc.** This atomicity enables precise linking and reuse.

## Contents

*   Focused `.md` notes, each covering **one specific thing** (e.g., `[[Regression]]`, `[[Confounding]]`).

## Workflow

1.  **Create:** New note for each distinct concept. Use a clear, precise title.
2.  **Define & Explain:** Use the `[[90 Meta/Templates/T - Atomic Note.md]]` template.
3.  **LINK!:** Crucial step. Use `[[Wikilinks]]` extensively to connect related concepts.
4.  **Add Examples/References:** Illustrate the concept and cite sources from `[[30 Resources/README|30 Resources]]`.
5.  **Use Aliases:** Add alternative names/acronyms in the frontmatter.
6.  **Review Auto-Links:** Check the Dataview block (requires plugin) at the bottom.

## Using the Template (`T - Atomic Note.md`)

This template structures your thinking about a single concept.

*   **YAML Frontmatter:**
	*   `subject`: Add a list of subjects you think it'll belong to
    *   `aliases: []`: **Crucial.** Add alternative names, synonyms, acronyms (e.g., `[DAG, Directed Acyclic Graph]`). This allows you to link using `[[DAG]]` and still find the note. Think about how *you* might search for or link to this concept later.
    *   `tags: [concept]`: The base tag identifies this as a core concept note. **Add TYPE or here**, *not subject tags*.
        *   Good examples: `#definition`, `#theorem`, `#method`, `#person`, `#question`.
        *   **AVOID:** `#statistics`, `#causal-inference`. Subject categorization is handled by linking *from* the relevant `[[20 MOCs/README|MOC]]`. Using subject tags here creates noise and redundancy.
	*   `status`: [state]
		*  Good examples: `#stub` (needs more work), `#WIP`, `#review`, `#complete`.
    *   `created`/`updated`: Auto-timestamps (requires plugin).
*   **`# {{title}}`**: The main heading. Should match the filename and be the precise name of the concept.
*   **`## Summary/Definition`**: A concise (1-3 sentence) definition or summary of the core idea. Write this clearly, as if explaining it to someone else (or your future self!).
*   **`## Explanation`**: Elaborate on the summary. Provide details, context, nuances, mechanisms, formulas, etc. **Link heavily** using `[[Wikilinks]]` to other Atomic Notes mentioned here. This is where you build the connections! If explaining Regression, link to `[[Linear Algebra]]`, `[[P-value]]`, `[[Hypothesis Testing]]`, etc., as you mention them.
*   **`## Examples`**: Concrete examples that illustrate the concept. These make abstract ideas easier to grasp.
*   **`## References`**: Link *specifically* to the notes in `[[30 Resources/README|30 Resources]]` where you learned about this concept (e.g., `Derived from: [[Book - Modern Epidemiology (Rothman)]]`).
*   **`#### Linked Concepts (Auto-Generated)`**: **Requires Dataview plugin.** This section dynamically lists outgoing wikilinks *from the body of this note* that point to files inside the `10 Atomic Notes` folder. It's a useful check to see the connections you've made. **You don't edit this section directly.**

**Things to Look Out For:**

*   **Atomicity:** Does this note *really* cover only one distinct idea? If it branches significantly, consider splitting it into multiple notes.
*   **Linking:** Are you linking relevant concepts *as you explain them*? The Explanation section should be rich with `[[Wikilinks]]`. Don't just rely on the auto-generated list at the bottom.
*   **Aliases:** Did you add common alternative names or acronyms? This drastically improves linking and discoverability.
*   **Tagging Discipline:** Stick to type/status tags. Avoid redundant subject tags.

## Key Connections

