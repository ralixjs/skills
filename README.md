# ralixjs/skills

A collection of **agent-ready skills** written as Markdown guides to help AI coding agents produce consistent, high-quality output—independent of the platform (GitHub Copilot, Cursor, Claude, etc.).

Each skill is designed to be *dropped into* your agent’s “skills” / “memory” / “knowledge base” system and used as an execution guide (conventions, patterns, examples, do’s & don’ts).

---

## Skills in this repository

### `ralix-rails`
Build structured frontend code in **Ruby on Rails** projects using the **Ralix** microframework.

Use it when creating or refactoring:

- Route-based **page controllers**
- Reusable **components** (with lifecycle hooks)
- **Templates** (HTML string functions)
- DOM / events / navigation / AJAX via **Ralix helpers**
- Integrations with **Rails UJS** and **Turbolinks/Turbo**

Source: `ralix-rails/SKILL.md`

---

## Repository structure

Each top-level folder represents a skill:

- `ralix-rails/`
  - `SKILL.md` — the full skill specification and guide (frontmatter + documentation)

This layout is intentionally simple so different platforms can ingest it easily.

---

## How to use these skills (platform-agnostic)

You can use this repo in any of the following ways:

1. **Copy/paste a skill** (`SKILL.md`) into your agent’s “skills” or “system prompt” area.
2. **Sync the repository** and let your agent load skills from disk.
3. **Index the Markdown** in your RAG/knowledge-base pipeline (recommended for larger sets of skills).

### Recommended ingestion rule
Treat each `*/SKILL.md` as a standalone unit:
- The YAML frontmatter is metadata (name, description, scope).
- The body contains the operational guide and examples.

---

## Contributing a new skill

PRs are welcome. To add a new skill:

1. Create a new folder (example: `my-skill/`)
2. Add a `SKILL.md` with:
   - YAML frontmatter (`name`, `description`, etc.)
   - sections like: **When to use**, **Architecture**, **Examples**, **Best practices**, **Common pitfalls**
3. Keep examples:
   - practical and copyable
   - consistent in style (naming, folder structure, conventions)
   - explicit about assumptions and constraints

---

## License

MIT. See `LICENSE`.
