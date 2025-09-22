# Domain, UI, and Infrastructure Boundaries

This document describes the boundaries between the main architectural layers of the Simple Genealogy Application.

## Domain Layer
- Contains all core business logic and rules for genealogy data.
- Defines entities: Individual, Relationship, Document, Photo, etc.
- Handles validation, data integrity, and support for non-traditional family structures.
- No dependencies on UI or infrastructure.

## UI Layer
- Implements the desktop user interface.
- Responsible for data entry forms, pedigree tree visualization, navigation, and user interactions.
- Communicates with the domain layer via well-defined interfaces.
- Handles presentation logic only; no business rules.

## Infrastructure Layer
- Manages data persistence (local storage), import/export (GEDCOM), and file system access.
- Provides services for saving/loading data, attaching documents/photos, and privacy controls.
- Exposes interfaces used by the domain and UI layers, but does not contain business or presentation logic.

## Layer Interaction
- UI interacts with the domain layer for all business operations.
- Domain layer requests data persistence or external services via infrastructure interfaces.
- Infrastructure implements the actual storage, import/export, and file access.

---
This separation ensures modularity, testability, and maintainability.