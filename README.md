# Zettelkasten Skills for Obsidian

An AI-augmented framework for managing a "Second Brain" in Obsidian using the Zettelkasten method. This project provides a set of specialized skills for AI agents (like Claude) to act as a **Vault Warden**, helping you automate the creation, linking, and quality assurance of atomic notes.

## 🧠 Core Philosophy

The Zettelkasten method, popularized by Niklas Luhmann, is a system for personal knowledge management that emphasizes **Atomicity** (one idea per note) and **Connectivity** (dense semantic linking). 

This project transforms your AI agent into a "Cognitive Processor" for your local Obsidian vault, reducing the clerical friction of maintaining a functional Zettelkasten.

## 🛠️ Key Skills

### ⚗️ Distill (Ingest)
Convert raw text or URLs into atomic Obsidian notes.
- **Decomposes** complex arguments into single propositions.
- **Rewrites** content to demonstrate understanding (Feynman Technique).
- **Populates** aliases and tags for better searchability.

### 🕸️ Weave (Link)
Integrate new notes into your existing graph.
- **Scans** context for semantic overlaps.
- **Suggests** direct and analogous connections.
- **Justifies** every link with a specific reason.

### 🔍 Critique (Quality Assurance)
Maintain vault hygiene and note standards.
- **Evaluates** notes against the Obsidian Quality Rubric.
- **Checks** for atomicity, specific titling, and frontmatter validity.
- **Refines** weak notes to meet the "Atomic Standard."

### 🗺️ Map (Visualize)
Visualize the local neighborhood of any topic.
- **Generates** Mermaid.js code blocks (flowcharts or mindmaps).
- **Links** nodes to exact filenames in your vault.

## 📋 Obsidian Standards

To ensure seamless integration, all outputs follow strict formatting rules:
- **Wikilinks:** Uses `[[filename]]` for all internal links.
- **Callouts:** Uses Obsidian callouts (e.g., `> [!INFO]`) for metadata.
- **Frontmatter:** Every note starts with a YAML block containing `id`, `aliases`, `tags`, and `date`.
- **Naming:** Uses `kebab-case-declarative-titles.md` for filenames.

## 🚀 Getting Started

### Method A: Claude CLI (Recommended)
Run the Claude CLI directly in your Obsidian vault root to allow it to read and write files in real-time.
1. Place `zettelkasten/SKILL.md` (or the contents of `zettelkasten.skill`) into your vault.
2. Activate the skill in your chat.
3. Use triggers like "Distill this article" or "Critique my draft note."

### Method B: Claude Projects (Web)
1. Create a new Project in the Claude.ai web interface.
2. Upload the `zettelkasten/SKILL.md` to the Project Knowledge base.
3. Paste the contents of `SKILL.md` into the Project Instructions.

## 📄 File Structure

- `zettelkasten/SKILL.md`: The core instruction set and skill definitions.
- `A Comprehensive Framework...md`: Detailed theoretical background and implementation guide.
- `zettelkasten.skill`: Binary/packaged version of the skill for supported platforms.

## 📜 License

[Specify License if applicable, e.g., MIT]
