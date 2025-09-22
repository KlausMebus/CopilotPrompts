# Architecture Decision Record: Modular Layered Architecture

## Status
Accepted

## Context
The Simple Genealogy Application must be maintainable, testable, and extensible. It must support privacy, local storage, and classic desktop workflows. The team has experience with F# and C#.

## Decision
- Use a modular, layered architecture:
  - **Domain Layer:** All business logic, validation, and core entities.
  - **UI Layer:** Desktop user interface, presentation logic only.
  - **Infrastructure Layer:** Data persistence, import/export, file system access.
- Each layer communicates only via well-defined interfaces.
- Domain logic is isolated from UI and infrastructure for testability.
- Use open standards (GEDCOM) for data exchange.

## Consequences
- Clear separation of concerns and responsibilities.
- Easier to test and maintain each layer independently.
- Supports future extensibility (e.g., new UI or storage backends).
- Onboarding is easier for new developers due to clear structure.

---
Created: 2025-09-22
