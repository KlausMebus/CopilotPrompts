---
mode: agent
tools: ['createFile', 'search', 'fetch']
---

# Create an Overall Implementation Plan

## Context

You are tasked with creating a comprehensive, but **high-level** implementation plan for the application.

There are documents in the `docs` folder you must use as references. These documents provide essential information about the application's core idea, product requirements, and which technical principles to follow.

The naming convention for the documents is as follows:
- [Name]-[Version].md where the [Version] starts from 0001 and increments for each new version of the document.

**Always** use the latest version of each document.

The documents are:
- Idea document: `idea-xxxx.md` 
- Product Requirements Document (PRD): `prd-xxxx.md`
- Technical Principles: `tech-principles-xxxx.md`

## Instructions
1. Carefully read the above documents to understand the application's core idea, product requirements, and guiding technical principles.
2. Before finalizing your plan, use a checklist to ensure every technical principle from the latest technical principles document is mapped to a concrete action, deliverable, or recurring task in the plan. For each principle, ask: “Is this reflected as a concrete task or deliverable in every relevant phase?”
3. Keep in mind the following while creating the plan:
   - The plan should be high-level and not get bogged down in implementation details.
   - Focus on major phases, key deliverables, dependencies, and critical tasks.
   - Consider risks and open questions that may impact the plan.
4. Synthesize an actionable, step-by-step plan for building the application. 
    - Make sure to cover all critical aspects needed for a successful implementation.
    - Make sure to follow the technical principles provided.
    - Your plan should include:
        - Major phases or milestones
        - Key deliverables for each phase
        - Dependencies and prerequisites for each phase
        - Major tasks to be completed in each phase to ensure successful delivery of key deliverables
        - Any critical risks or open questions
    - Make sure that the dependencies between phases are clear and logical.
        - For the first phase, there should be no dependencies or at least only very trivial ones.
            - Architectural design is NOT a trivial dependency and cannot be a dependency for Phase 1.
            - Scaffolding or setting up the project structure is not a trivial dependency and cannot be a dependency for Phase 1.
        - Each subsequent phase should depend on the successful completion of the previous phase(s).
5. Present the plan in a clear, structured format (e.g. numbered list, table, or roadmap).
6. Ensure the plan is practical and can guide a team or a person from concept to launch.

## Output Guidelines
- Output must be in valid Markdown.
- Use clear, concise language.
- Reference external standards or documentation where relevant.
- Save the overall plan document as `plan-xxxx.md` (where `xxxx` is an ID which can be incremented if additional versions are created) in the `docs` folder.
- The final document must include both the **current date and time** in the timestamp at the end (e.g., `Created on: 21-09-2025 - 14:37` but showing the actual current date and time).

### Output Format (Strict Template)

- Make sure to follow the exact structure and headings as shown below.
- Make sure to use valid Markdown syntax.
- Make sure to include the creation date and time at the end of the document.

```markdown
# Implementation Plan

## 1. Overview
Brief summary of the application and its goals (1-2 sentences).

## 2. Major Phases & Milestones

### 2.1 Phase 1: [Phase Name]
- **Description:** Brief description of this phase.
- **Key Deliverables:** List of key deliverables for this phase.
- **Dependencies:** List of dependencies for this phase.
- **Major tasks:** List of major tasks to be completed in this phase to ensure successful delivery of key deliverables.

### 2.2 Phase 2: [Phase Name]
- **Description:** Brief description of this phase.
- **Key Deliverables:** List of key deliverables for this phase.
- **Dependencies:** List of dependencies for this phase.
- **Major tasks:** List of major tasks to be completed in this phase to ensure successful delivery of key deliverables.

### 2.N Phase N: [Phase Name]
- **Description:** Brief description of this phase.
- **Key Deliverables:** List of key deliverables for this phase.
- **Dependencies:** List of dependencies for this phase.
- **Major tasks:** List of major tasks to be completed in this phase to ensure successful delivery of key deliverables.

## 3. Risks & Open Questions
- List critical risks
- List open questions or assumptions

## 4. Alignment with Technical Principles
- Bullet points showing how the plan aligns with the technical principles

## 5. References
- List relevant sections from documents provided in the `docs` folder.
- List relevant references from websites, articles, or other resources if applicable.

---
Created on: [Date] - [Time]
```

