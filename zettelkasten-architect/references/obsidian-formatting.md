# Obsidian Formatting Rules & Data Standards

To ensure compatibility with Obsidian's features and the Zettelkasten method, the following standards must be strictly enforced.

## 1. Links & Connections
*   **Wikilinks:** ALWAYS use `[[filename]]` for internal links.
    *   *Incorrect:* `[link title](filename.md)` or `[link title](url)` (for internal files).
    *   *Correct:* `[[my-concept-note]]` or `[[my-concept-note|custom display text]]`.
*   **Link Justification:** Every link in the "Connections" section must have a reason appended.
    *   *Format:* `- [[linked-note]] - Reason for connection (e.g., "Supports argument", "Provides counter-example", "Analogous structure").`

## 2. Callouts
Use Obsidian-flavored callouts for metadata, summaries, or specific content types.
*   **Syntax:** `> [!TYPE] Title`
*   **Standard Types:**
    *   `> [!INFO]` - General information.
    *   `> [!SUMMARY]` - Summaries.
    *   `> [!QUOTE]` - Verbatim quotes.
    *   `> [!TODO]` - Action items.

## 3. Math & Diagrams
*   **Math:** Use LaTeX enclosed in `$` for inline math ($E=mc^2$) and `$$` for block math.
*   **Diagrams:** Use Mermaid.js code blocks for graphs and charts.
    ```mermaid
    graph TD
    A[Start] --> B{Decision}
    ```

## 4. Frontmatter (YAML)
Every note MUST start with a YAML frontmatter block enclosed in `---`.

### Standard Properties
| Field | Format | Purpose |
| :--- | :--- | :--- |
| `id` | `YYYYMMDDHHmm` | Unique ID for robust linking. |
| `aliases` | `['term 1', 'term 2']` | Allows "Unlinked Mentions" to find connections. |
| `tags` | `[topic/subtopic]` | Hierarchical tags for filtering. |
| `date` | `YYYY-MM-DD` | Creation date. |
| `cssclass`| `cards` | (Optional) For "Minimal" theme card views. |

## 5. File Naming
*   **Convention:** `kebab-case-declarative-title.md`
*   **Goal:** Specificity.
    *   *Bad:* `inflation.md`
    *   *Good:* `inflation-causes-instability.md`
