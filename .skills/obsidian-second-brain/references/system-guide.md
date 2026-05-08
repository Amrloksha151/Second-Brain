# Second Brain System Guide (PARA + CS)

This document defines the organizational structure and rules for the Obsidian Second Brain.

## 📁 Folder Structure

- **00 Inbox**: For quick captures and unprocessed notes.
- **10 Projects**: Active endeavors with a deadline (e.g., `Build Gemini Skill`, `Thesis Implementation`).
- **20 Areas**: Ongoing responsibilities with a standard to be maintained (e.g., `Health`, `Finances`, `System Architecture`, `Software Engineering`).
- **30 Resources**: Interests and reference material (e.g., `Rust Language`, `Distributed Systems Papers`, `Cookbook`).
- **40 Archives**: Completed projects or inactive interests.
- **99 System**: Templates, Attachments, and Scripts.

## 📜 Organizational Rules

1.  **Atomic Notes**: Each note should focus on one concept or project.
2.  **YAML First**: Every note MUST have a YAML frontmatter block for metadata.
3.  **WikiLinks**: Always link related notes using `[[Note Name]]`. If a note is mentioned, link it.
4.  **Date Standard**: Use `YYYY-MM-DD` for all dates.
5.  **Project Life Cycle**:
    - Creation -> `10 Projects/Project Name/Project Name.md`
    - Completion -> Move folder to `40 Archives/YYYY/Project Name`

## 💻 CS Specializations

- **Code Snippets**: Should be stored in `30 Resources/Code Snippets` or within the relevant Project folder. Always include the language tag.
- **Concepts**: Fundamental CS concepts (e.g., `Paxos`, `B-Trees`) live in `30 Resources/Concepts`.
- **People**: Technical contacts should be stored in `20 Areas/Network/People`.
