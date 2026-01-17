# Zettelkasten Skills for Obsidian

This repository contains specialized "skills" for AI agents (specifically Claude) to help manage, architect, and maintain a Zettelkasten knowledge base within Obsidian.

## Available Skills

### `zettelkasten-architect`
A comprehensive "Cognitive Processor" for your Second Brain. It acts as a "Vault Warden" to ensure note quality, atomicity, and connectivity.

*   **Location:** `zettelkasten-architect/`
*   **Core Role:** Transforms raw input into atomic, permanent notes and connects them to your existing vault.
*   **Key Commands:**
    *   `/distill`: Decompose raw text into atomic Permanent Notes with proper metadata.
    *   `/weave`: Find semantic connections between a new note and your existing vault.
    *   `/critique`: Grade notes against strict Zettelkasten standards (atomicity, linking, formatting) and rewrite them if they fail.
    *   `/graph`: Generate Mermaid.js visualizations of local note neighborhoods.

## Usage

1.  **Install:** Copy the `zettelkasten-architect` folder to your agent's skill directory.
2.  **Configuration:** Ensure your Obsidian vault follows the standards defined in `zettelkasten-architect/references/obsidian-formatting.md`.
3.  **Trigger:** Use natural language or the specific commands (e.g., "Distill this article", "Critique this note") to activate the skill.

## Standards & Philosophy

This project adheres to:
*   **Atomicity:** One idea per note.
*   **Obsidian Flavored Markdown:** Strict adherence to wikilinks `[[...]]`, callouts `> [!INFO]`, and YAML frontmatter.
*   **Link Justification:** Every link must have a stated reason for its existence.
