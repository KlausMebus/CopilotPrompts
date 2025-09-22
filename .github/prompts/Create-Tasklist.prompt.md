---
mode: agent
tools: ['createFile', 'search', 'fetch']
---

# Create Task List

## Context
You are tasked with generating a detailed, actionable task list for the application based on the high-level implementation plan and supporting documents.
The target audience for this task list is a junior development team that will use it to guide their work.

The following documents are available in the `docs` folder and must be used as references:
- The implementation plan: `plan-xxxx.md` (where `xxxx` is the latest version)
- The idea document: `idea-xxxx.md`
- The product requirements document (PRD): `prd-xxxx.md`
- The technical principles: `tech-principles-xxxx.md`

**Always use the latest version of each document.**

## Instructions

1. Read the latest implementation plan and supporting documents to understand the application's goals, requirements, and technical principles.
2. Break down each major task or deliverable in the plan into smaller, actionable tasks and subtasks.
3. Structure the output as a markdown checklist, using bullet lists and markdown checkboxes (`- [ ]`).
    - Each phase should be a section header (e.g., `## Phase 1: ...`).
    - Each major task should be a top-level checkbox with a unique number (e.g., `- [ ] 1. ...`).
    - Each subtask should be a nested checkbox with a decimal number (e.g., `- [ ] 1.1 ...`).
    - Use up to three levels of numbering if needed.
4. Ensure that the numbering is explicit and consistent for easy reference.
5. The task list should be comprehensive, actionable, and practical for guiding implementation.
6. Reference the plan, PRD, idea, and technical principles to ensure all requirements and constraints are covered.
7. Save the output as `tasklist-xxxx.md` (incrementing the version as needed) in the `docs` folder.
8. Include the current date and time at the end of the document (e.g., `Created on: 21-09-2025 - 14:37` but using the actual current date and time).

## Output Guidelines

- Output must be in valid Markdown.
- Use clear, concise language.
- Use markdown checkboxes for all tasks and subtasks.
- Use explicit numbering for all tasks and subtasks.
- Use section headers for each phase.
- The output should be ready to use as a project task board or checklist.
- Include a references section listing the documents used.
- End with a timestamp.

### Output Format (Strict Template)

```markdown
# Detailed Task List for Implementation Plan

## Introduction
Briefly describe the purpose of the task list and its source documents.

---

## Phase 1: [Phase Name]
- [ ] 1. [Major Task]
  - [ ] 1.1 [Subtask]
  - [ ] 1.2 [Subtask]
    - [ ] 1.2.1 [Sub-subtask]
  ...
- [ ] 2. [Major Task]
  ...

## Phase 2: [Phase Name]
...

## References
- [plan-xxxx.md](plan-xxxx.md)
- [idea-xxxx.md](idea-xxxx.md)
- [prd-xxxx.md](prd-xxxx.md)
- [tech-principles-xxxx.md](tech-principles-xxxx.md)

---
Created on: [Date] - [Time]
```
