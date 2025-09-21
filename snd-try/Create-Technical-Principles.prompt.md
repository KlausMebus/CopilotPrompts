# Create Technical Principles

## Purpose
This prompt is designed to help you define the technical principles and architectural guidelines that an application must adhere to. It is intended for use alongside an existing idea description and product requirements document, to ensure technical alignment and consistency throughout the development process.


## Instructions
- Start by gathering context from the idea description and product requirements document.
    - They are typically found in files named `idea-xxxx.md` and `prd-xxxx.md`, where `xxxx` is the ID. Use the largest ID for each type of document if multiple exist (note that the idea ID and PRD ID may differ).
- Use this prompt to clarify and document the technical principles for your application.
- Start by asking clarifying questions about technical constraints, preferences, and priorities using the Technical Question Process below.
- Consider the following aspects (add, remove, or modify as needed):
   - Programming languages and frameworks
   - Target platforms (web, desktop, mobile, CLI, etc.)
   - Architectural style (e.g., monolith, microservices, modular)
   - Programming paradigms (functional, object-oriented, procedural, or hybrid)
   - Allowed or preferred styles in different layers or modules
   - Dependency management and third-party libraries
   - Code quality standards (linting, formatting, testing, documentation)
   - Security and privacy requirements
   - Performance and scalability expectations
   - Extensibility and maintainability
   - Interoperability and integration constraints
   - Tooling and development environment
   - Version control and branching strategy
   - Deployment and release process
- For each principle, provide a clear rationale and, if relevant, examples or references.
- If there are trade-offs or exceptions, document them explicitly.
- Use the workflow steps below to guide your process.

## Technical Question Process

- Before defining technical principles, ask clarifying questions to fully understand technical constraints, preferences, and priorities.
- Use a numbered list for questions, and do not ask more than 3 at a time.
- **You must repeat this step until all major technical areas (see checklist below) are addressed or confirmed as not relevant.**
- After each round, summarize which areas have been covered and which remain. If any area is unclear, ambiguous, or missing, explicitly ask for clarification before proceeding.
- Document any open questions or uncertainties in the technical principles document if they cannot be resolved immediately.

**Technical Areas Checklist:**
- Programming languages
- Frameworks
- Target platforms (web, desktop, mobile, CLI, etc.)
- Architectural style (e.g., monolith, microservices, modular)
- Programming paradigms (functional, object-oriented, procedural, or hybrid)
- Allowed or preferred styles in different layers or modules
- Test strategies (unit, integration, end-to-end)
- Data storage and management
- Internationalization/localization requirements
- Documentation process and standards
- Dependency management and third-party libraries
- Code quality standards (linting, formatting, testing, documentation)
- Security and privacy requirements
- Performance and scalability expectations
- Extensibility and maintainability
- Interoperability and integration constraints
- Tooling and development environment
- Version control and branching strategy
- Deployment and release process

**Process Guidance:**
1. In each iteration, select up to 3 technical areas from the checklist that are not yet fully clarified and ask focused questions about them.
2. After each round, provide a summary table or checklist showing which areas are clarified, which are open, and which are not relevant.
3. Continue doing a round until all areas are either clarified, marked as not relevant, or explicitly deferred.
4. Ask for any additional technical areas that may be relevant but are not listed. And ask clarifying questions about them if needed.


## Workflow Steps
1. **Review Context**
   - Review the idea description and product requirements document.
   - Identify any technical constraints or preferences already stated.
2. **Ask Clarifying Technical Questions**
   - Use the Technical Question Process to ask clarifying questions about technical constraints, preferences, and priorities. Limit to 4 questions per iteration, and repeat for at least 2 iterations or at least until all technical areas in the checklist are addressed.
   - After each round, summarize which technical areas have been clarified and which remain open.
   - Document answers and any remaining uncertainties.
3. **Define Core Principles**
   - List and describe the core technical principles for the application.
   - For each, specify where and how it applies (e.g., "use functional programming for data processing modules, OOP for UI").
4. **Clarify Allowed Variations**
   - Document any areas where different styles or technologies are allowed or required.
   - Note any exceptions or special cases.
5. **Rationale and Trade-offs**
   - For each principle, explain the reasoning and any trade-offs involved.
6. **Finalize and Review**
   - Ensure all principles are well-defined, clearly articulated and not contradictory.
   - Verify that the document includes both the current date and time in the timestamp at the end.
   - Present the technical principles document for review.
   - Revise as needed based on feedback.

## Output Guidelines
- Output must be in valid Markdown.
- Use clear, concise language.
- Reference external standards or documentation where relevant.
- Save the technical principles document as `tech-principles-xxxx.md` (where `xxxx` is an ID which can be incremented if additional versions are created) in the `docs` folder.
- The final document must include both the current date and time in the timestamp at the end (e.g., `Created on: 21-09-2025 - 14:37`).

### Strict Document Format
Every technical principles document must follow this structure:

```markdown
# Technical Principles for [Application Name] 

## 1. Context and Inputs
- **Idea Description:** (Reference to idea-xxxx.md)
- **Product Requirements:** (Reference to prd-xxxx.md)
- **Key Technical Constraints/Preferences:** (Summarize any known constraints or preferences)

## 2. Core Principles

### 2.1 Principle Name

- **Description:**  
   (What is the principle? State it clearly and concisely.)

- **Scope:**  
   (Where and how does it apply? E.g., “All backend modules”, “Only for UI components”, etc.)

- **Rationale:**  
   (Why is this principle important? What problem does it solve?)

- **Examples/References:** (Optional)  
   (Optional: Code snippets, links to standards, or documentation.)

- **Trade-offs/Exceptions:**  
   (Any known trade-offs, limitations, or exceptions to this principle.)

## 3. Allowed Variations and Exceptions (if any)
- Document any areas where different styles or technologies are allowed or required.
- Note any exceptions or special cases.

## 4. Defferred Questions or Uncertainties (if any)
- Document any open questions or uncertainties that could not be resolved immediately.

---
Created on: [Date] - [Time]
```


