---
name: obsidian-second-brain
description: Manage an Obsidian Second Brain using PARA methodology for CS professionals. Use when creating projects, capturing ideas, saving code snippets, or organizing research papers and technical contacts.
---

# Obsidian Second Brain Manager

This skill transforms Gemini CLI into a specialized assistant for managing your Obsidian-based "Second Brain". It uses the PARA method (Projects, Areas, Resources, Archives) and is optimized for Computer Science professionals.

## 📁 System Architecture

The brain is organized into:
- `00 Inbox`: Raw captures.
- `10 Projects`: Active work.
- `20 Areas`: Standards and ongoing responsibilities.
- `30 Resources`: Knowledge base (Concepts, Snippets, Papers).
- `40 Archives`: Cold storage.

## 🛠️ Commands & Workflows

### 1. Capture & Inbox
- **Command**: `brain capture <thought>`
- **Action**: Append to `00 Inbox/Inbox.md` or create a new note in `00 Inbox/` if the thought is substantial.
- **Workflow**: Always include a `#thought` tag and the creation date.

### 2. Project Management
- **Command**: `brain project new "<Name>"`
- **Action**: 
    1. Create folder `10 Projects/<Name>`.
    2. Create `10 Projects/<Name>/<Name>.md` using `Project.md` template.
- **Milestone Update**: `brain milestone "<Task>" for "<Project>"`
    - Find the project file and append the task to the Milestones section.

### 3. CS Knowledge Base
- **Concept**: `brain concept add "<Title>"`
    - Create in `30 Resources/Concepts/` using `CS-Concept.md`.
- **Snippet**: `brain snippet save "<Title>"`
    - Create in `30 Resources/Code Snippets/` using `Code-Snippet.md`.
- **Research**: `brain research add "<Paper Title>"`
    - Create in `30 Resources/Research/` using `Paper.md`.

### 4. Networking
- **Person**: `brain person add "<Name>"`
    - Create in `20 Areas/Network/People/` using `Person.md`.

## 📜 Core Rules for the Agent

1.  **Always Search First**: Before creating a note, search if it already exists to avoid duplicates.
2.  **WikiLink Everything**: If you mention a concept, project, or person that likely exists in the brain, wrap it in `[[Double Brackets]]`.
3.  **YAML Integrity**: Never omit the YAML frontmatter. Use the provided templates in `assets/templates/`.
4.  **Date Format**: Always use `YYYY-MM-DD`.
5.  **Context Awareness**: If working on a file in the project, offer to save snippets or notes related to that file into the Brain.

## 🧠 Brain Review
- **Inquiry**: "What's on my plate?" or `brain status`.
- **Action**: List files in `10 Projects/` and un-triaged notes in `00 Inbox/`.

## 📚 Reference Material
For detailed organization rules, see [system-guide.md](../references/system-guide.md).
