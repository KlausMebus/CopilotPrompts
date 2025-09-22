# Technical Principles for Simple Genealogy Application

## 1. Context and Inputs
- **Idea Description:** [idea-0002.md](idea-0002.md)
- **Product Requirements:** [prd-0002.md](prd-0002.md)
- **Key Technical Constraints/Preferences:**
  - .NET as the main framework
  - F# for the domain model, C# for UI and application control
  - Modular monolith architecture
  - Functional programming preferred for domain logic, OOP for UI/app control
  - Use NuGet and prefer OSS from well-known organizations
  - Incremental development approach
  - Local desktop application, privacy by default
  - VS Code and Git/GitHub for development
  - Import/export via GEDCOM is essential

## 2. Core Principles

### 2.1 Language and Framework
- **Description:**  Use .NET as the primary framework, F# for domain logic, and C# for UI and application orchestration.
- **Scope:**  All application layers.
- **Rationale:**  Leverages strengths of both languages: F# for functional, robust domain modeling; C# for UI and integration with .NET desktop frameworks.
- **Trade-offs/Exceptions:**  Some libraries may require C# wrappers for F# interop.

### 2.2 Architecture
- **Description:**  Modular monolith with clear separation between domain, UI, and infrastructure.
- **Scope:**  Entire application structure.
- **Rationale:**  Supports maintainability, testability, and incremental development without microservices complexity.
- **Trade-offs/Exceptions:**  No external plugin support in v1.

### 2.3 Programming Paradigm
- **Description:**  Prefer functional programming for domain logic; use OOP where required by UI frameworks or libraries.
- **Scope:**  Domain model (functional), UI/app control (OOP).
- **Rationale:**  Functional paradigm improves correctness and testability; OOP fits UI frameworks and event-driven code.
- **Trade-offs/Exceptions:**  Hybrid approach may require careful interface design.

### 2.4 Dependency Management
- **Description:**  Use NuGet for dependencies; prefer open-source libraries from reputable organizations.
- **Scope:**  All dependencies.
- **Rationale:**  Ensures reliability, maintainability, and legal clarity.
- **Trade-offs/Exceptions:**  Avoid GPL or restrictive licenses.

### 2.5 Code Quality and Testing
- **Description:**  Enforce code formatting, static analysis, and code review. Use unit, integration, and end-to-end tests as part of incremental development.
- **Scope:**  All code and modules.
- **Rationale:**  Maintains high code quality and reduces defects.
- **Trade-offs/Exceptions:**  Some manual testing may be needed for UI.

### 2.6 Documentation
- **Description:**  Maintain both inline code comments and external documentation (e.g., markdown, diagrams).
- **Scope:**  All code and major design decisions.
- **Rationale:**  Supports maintainability and onboarding.

### 2.7 Security and Privacy
- **Description:**  Local data storage by default; follow secure coding practices.
- **Scope:**  All data and code.
- **Rationale:**  Minimizes privacy risks and attack surface.
- **Trade-offs/Exceptions:**  No cloud or telemetry in v1.

### 2.8 Performance and Scalability
- **Description:**  Application should perform smoothly with up to 1,000 people per dataset.
- **Scope:**  All features and data operations.
- **Rationale:**  Ensures usability for target audience.

### 2.9 Extensibility and Maintainability
- **Description:**  Modular code, clear separation of concerns, no external plugin support in v1.
- **Scope:**  All modules.
- **Rationale:**  Supports future growth and easier maintenance.

### 2.10 Interoperability
- **Description:**  Support import and export via GEDCOM.
- **Scope:**  Data import/export features.
- **Rationale:**  Ensures compatibility with other genealogy tools.

### 2.11 Tooling and Development Environment
- **Description:**  Use VS Code and Git/GitHub for development and version control.
- **Scope:**  All development activities.
- **Rationale:**  Supports modern, collaborative workflows.

### 2.12 Version Control and Branching
- **Description:**  Use Git/GitHub; branching strategy to be determined.
- **Scope:**  All code.
- **Rationale:**  Enables collaboration and code history.

### 2.13 Deployment and Release
- **Description:**  Deployment and release process to be defined later.
- **Scope:**  All releases.
- **Rationale:**  Allows flexibility as requirements become clearer.

## 3. Allowed Variations and Exceptions (if any)
- OOP is allowed in UI and application control layers.
- No external plugin support in v1.
- Branching and deployment strategies are open for future definition.

## 4. Deferred Questions or Uncertainties (if any)
- Branching strategy for version control is not yet defined.
- Deployment and release process is not yet defined.

---
Created on: 22-09-2025 - 00:00
