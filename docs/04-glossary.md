# 04 — Glossary

## Document Purpose

This document defines the shared glossary baseline for KUNNA.

The glossary was initially created during the **I1 — Inception Package** and is maintained as the project progresses through **I2 — Elaboration** and later lifecycle work.

The purpose of this artifact is to provide a shared vocabulary across:

- Product vision.
- User goals.
- Use cases.
- Supplementary requirements.
- Domain modeling.
- Analysis and design.
- Design decisions.
- Progressive Java implementation.

The glossary should reduce ambiguity without attempting to define every possible project term in advance.

## Language Rule

KUNNA follows a hybrid language strategy:

- Technical language: English.
- Product and domain language: Spanish when useful.
- Repository artifacts: mainly English.
- User-facing content and Colombian domain examples: mainly Spanish.

This glossary may include both English and Spanish terms when that improves clarity.

## Core Product Terms

| Term                         | Spanish / Domain Equivalent        | Definition                                                                                                                                                |
| ---------------------------- | ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| KUNNA                        | KUNNA                              | Digital product concept intended to support caregivers with accessible information about children's rights, positive parenting, and daily care practices. |
| Product                      | Producto                           | The digital experience or system being designed and progressively implemented.                                                                            |
| Prototype                    | Prototipo                          | The original UX/UI concept created in Figma, used as an input to the current software engineering project.                                                |
| Software Engineering Project | Proyecto de ingeniería de software | The structured evolution of KUNNA through product reasoning, documentation, analysis, design, implementation, testing, and evidence.                      |
| Inception Package            | Paquete de Inicio                  | Initial set of artifacts that established the project vision, users, use cases, requirements, risks, plan, and decision baseline.                         |
| Product Vision               | Visión del producto                | High-level explanation of what KUNNA is intended to become, why it exists, who it may serve, and what outcomes it seeks.                                  |
| Product-First Approach       | Enfoque primero producto           | Strategy where problems, users, outcomes, and assumptions are considered before implementation decisions are committed.                                   |

## User and Actor Terms

| Term                  | Spanish / Domain Equivalent | Definition                                                                                                    |
| --------------------- | --------------------------- | ------------------------------------------------------------------------------------------------------------- |
| User                  | Usuario                     | Any person who interacts with KUNNA.                                                                          |
| Actor                 | Actor                       | A role that interacts with the system in a use case model.                                                    |
| Caregiver             | Cuidador / cuidadora        | Main user role. A person involved in supporting, protecting, educating, or caring for a child in daily life.  |
| Mother                | Madre                       | A caregiver role represented in the product domain.                                                           |
| Father                | Padre                       | A caregiver role represented in the product domain.                                                           |
| Guardian              | Acudiente / tutor           | A person legally or practically responsible for a child.                                                      |
| Guest User            | Usuario invitado            | Provisional user variant that may access behavior without authentication.                                     |
| Registered Caregiver  | Cuidador registrado         | Provisional caregiver variant that may have a profile, saved content, preferences, or account-specific state. |
| Content Administrator | Administrador de contenido  | Possible future role responsible for creating, editing, or managing KUNNA content.                            |
| Primary Actor         | Actor primario              | The actor whose goal is fulfilled by a use case.                                                              |
| Supporting Actor      | Actor de soporte            | An external system or role that supports completion of a use case.                                            |

## Domain Terms

| Term               | Spanish / Domain Equivalent | Definition                                                                                                   |
| ------------------ | --------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Child              | Niño / niña                 | A person who is the subject of care, protection, rights, and parenting content.                              |
| Children           | Niñas y niños               | Children as the main protected population in the product domain.                                             |
| Child Rights       | Derechos de niñas y niños   | Rights and protections related to children. KUNNA may present this content in accessible language.           |
| Positive Parenting | Crianza positiva            | Parenting approach focused on respect, care, communication, guidance, protection, and non-violent practices. |
| Caregiving         | Cuidado                     | Daily actions related to supporting, protecting, educating, and accompanying a child.                        |
| Daily Care         | Cuidado diario              | Everyday child-care situations where caregivers may need guidance.                                           |
| Colombian Context  | Contexto colombiano         | Domain context related to Colombia, caregivers, child rights, institutions, and social realities.            |
| Sensitive Content  | Contenido sensible          | Content that must be treated carefully because it relates to children, rights, protection, or caregiving.    |

## Content Terms

| Term                | Spanish / Domain Equivalent    | Definition                                                                                                                      |
| ------------------- | ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| Content             | Contenido                      | Information that may be made available through KUNNA, such as articles, tips, audio, resources, or child-rights explanations.   |
| Content Item        | Pieza de contenido             | A single unit of content that may support one or more interactions depending on the selected product behavior.                  |
| Daily Tip           | Tip diario                     | Short practical content intended to provide caregivers with concise guidance.                                                   |
| Article             | Artículo                       | Longer content item that explains a topic in more detail.                                                                       |
| Resource            | Recurso                        | Material intended to support caregivers; it may be reusable or downloadable when the selected product scope requires it.        |
| Audio Content       | Contenido en audio             | Content represented or delivered in audio form when audio behavior is part of the product scope.                                |
| Category            | Categoría                      | Possible grouping used to organize content by topic, such as child rights, positive parenting, daily care, resources, or audio. |
| Search Result       | Resultado de búsqueda          | A content item returned when search behavior is supported and matches user-provided criteria.                                   |
| User-Facing Content | Contenido visible para usuario | Text, audio, labels, messages, or information shown directly to the caregiver.                                                  |

## Interaction Terms

| Term                      | Spanish / Domain Equivalent          | Definition                                                                                                                    |
| ------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| View Content              | Ver contenido                        | Candidate use case where a caregiver accesses or consults a content item.                                                     |
| View Daily Tip            | Ver tip diario                       | Candidate use case where a caregiver accesses a short daily parenting or caregiving tip.                                      |
| Browse Content Categories | Explorar categorías                  | Candidate use case where a caregiver navigates available content by topic or category.                                        |
| Search Content            | Buscar contenido                     | Candidate use case where a caregiver searches for content using criteria such as a keyword or topic.                          |
| Bookmark Content          | Guardar contenido / marcar contenido | Candidate use case where a caregiver marks content for later consultation.                                                    |
| View Saved Content        | Ver contenido guardado               | Candidate use case where a caregiver revisits previously saved content.                                                       |
| Play Audio Content        | Reproducir audio                     | Candidate use case where a caregiver accesses audio-based content.                                                            |
| Download Resource         | Descargar recurso                    | Candidate use case where a caregiver requests a resource for later use when download behavior is supported.                   |
| Share Content             | Compartir contenido                  | Candidate use case where a caregiver initiates sharing; external platform integration is not assumed unless required.         |
| Manage Profile            | Gestionar perfil                     | Candidate use case where profile information or preferences are managed if personalization becomes part of the product scope. |

## Requirements Terms

| Term                      | Spanish / Domain Equivalent | Definition                                                                                                                    |
| ------------------------- | --------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Requirement               | Requisito                   | A condition or capability that the system should satisfy once it has been accepted as part of the relevant scope.             |
| Functional Requirement    | Requisito funcional         | A requirement that describes what the system should do.                                                                       |
| Supplementary Requirement | Requisito complementario    | A cross-cutting requirement or constraint not fully described by one use case.                                                |
| Constraint                | Restricción                 | A limitation, rule, or condition that affects the project or solution.                                                        |
| Quality Attribute         | Atributo de calidad         | A characteristic such as usability, accessibility, reliability, security, performance, or maintainability.                    |
| Usability                 | Usabilidad                  | How easy and understandable the product is for caregivers.                                                                    |
| Accessibility             | Accesibilidad               | The degree to which the product can be used by people with different needs, abilities, or contexts.                           |
| Reliability               | Confiabilidad               | The ability of the system to behave consistently and predictably.                                                             |
| Security                  | Seguridad                   | Protection of data, access, and system behavior.                                                                              |
| Privacy                   | Privacidad                  | Responsible handling of user information and personal data.                                                                   |
| Performance               | Rendimiento                 | How efficiently or quickly the system responds under relevant conditions.                                                     |
| Maintainability           | Mantenibilidad              | How easy it is to understand, modify, test, and improve the project over time.                                                |
| Traceability              | Trazabilidad                | The ability to connect product reasoning, requirements, issues, decisions, code, tests, commits, pull requests, and evidence. |

## Analysis and Design Terms

| Term                         | Spanish / Domain Equivalent         | Definition                                                                                                        |
| ---------------------------- | ----------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Use Case                     | Caso de uso                         | Description of how an actor interacts with the system to achieve a goal.                                          |
| Use Case Model               | Modelo de casos de uso              | Collection of actors, candidate use cases, and relationships describing externally observable system behavior.    |
| User Goal                    | Objetivo de usuario                 | An outcome a user may want to accomplish with the product.                                                        |
| System Boundary              | Límite del sistema                  | The separation between what belongs inside KUNNA and what remains outside it.                                     |
| Domain Model                 | Modelo de dominio                   | Conceptual model that identifies important real-world concepts and relationships in the problem domain.           |
| UML                          | UML                                 | Unified Modeling Language, used selectively to represent software analysis and design visually.                   |
| System Sequence Diagram      | Diagrama de secuencia del sistema   | Diagram that shows interactions between an actor and the system for a use case scenario.                          |
| Operation Contract           | Contrato de operación               | Description of a system operation and relevant preconditions, postconditions, or state changes.                   |
| Object-Oriented Analysis     | Análisis orientado a objetos        | Process of understanding the problem domain using concepts, relationships, system behavior, and responsibilities. |
| Object-Oriented Design       | Diseño orientado a objetos          | Process of assigning software responsibilities to collaborating objects and classes.                              |
| GRASP                        | GRASP                               | Set of patterns and principles used to reason about responsibility assignment in object-oriented design.          |
| Architecture Decision Record | Registro de decisión arquitectónica | Document that records an important architecture or technical decision and its reasoning.                          |
| ADR                          | ADR                                 | Short form for Architecture Decision Record.                                                                      |

## GitHub Workflow Terms

| Term                | Spanish / Domain Equivalent | Definition                                                                                       |
| ------------------- | --------------------------- | ------------------------------------------------------------------------------------------------ |
| Repository          | Repositorio                 | GitHub project space that stores files, documentation, code, issues, pull requests, and history. |
| Issue               | Tarea / asunto              | Work item used to describe a task, problem, decision, requirement, or artifact to complete.      |
| Milestone           | Hito                        | Group of issues that belong to a specific project phase or goal.                                 |
| Project Board       | Tablero del proyecto        | Kanban-style board used to organize work by status.                                              |
| Backlog             | Pendiente                   | Work that has been identified but is not currently active.                                       |
| Ready               | Listo                       | Work sufficiently prepared to become active when capacity and sequencing allow it.               |
| In Progress         | En progreso                 | Work currently being developed.                                                                  |
| Review              | Revisión                    | Work waiting for review before being completed.                                                  |
| Done                | Terminado                   | Work completed and integrated.                                                                   |
| Branch              | Rama                        | Isolated line of work used to make changes before merging into `main`.                           |
| Main Branch         | Rama principal              | Stable branch where completed and reviewed work is integrated.                                   |
| Commit              | Commit                      | A saved change in Git history.                                                                   |
| Conventional Commit | Commit convencional         | Commit message style that clearly describes the type and purpose of a change.                    |
| Pull Request        | Solicitud de integración    | Request to merge changes from a branch into `main`.                                              |
| Merge               | Integración                 | Action of combining changes from a branch into another branch.                                   |
| Label               | Etiqueta                    | Classification used to organize issues and pull requests.                                        |
| Assignee            | Responsable                 | Person assigned to complete or manage an issue.                                                  |

## Project Artifact Terms

| Term                        | Spanish / Domain Equivalent         | Definition                                                                                       |
| --------------------------- | ----------------------------------- | ------------------------------------------------------------------------------------------------ |
| Artifact                    | Artefacto                           | A document, model, decision record, code file, test, or other project output.                    |
| README                      | README                              | Main repository document that explains the project to visitors.                                  |
| Vision Document             | Documento de visión                 | Artifact that defines the product idea, problem hypotheses, users, scope, and outcomes.          |
| User Goals Document         | Documento de objetivos de usuario   | Artifact that records candidate user goals and their current interpretation.                     |
| Use Case Model Document     | Documento de modelo de casos de uso | Artifact that records candidate actors, use cases, mappings, and behavioral relationships.       |
| Supplementary Specification | Especificación complementaria       | Artifact that documents relevant cross-cutting requirements and constraints.                     |
| Glossary                    | Glosario                            | Artifact that defines shared project and domain terminology.                                     |
| Risk List                   | Lista de riesgos                    | Artifact that identifies, prioritizes, and tracks project risks.                                 |
| Development Plan            | Plan de desarrollo                  | Artifact that defines lifecycle direction, iteration objectives, and development strategy.       |
| Development Framework       | Marco de desarrollo                 | Artifact that defines process, workflow, and working rules.                                      |
| AI Collaboration Policy     | Política de colaboración con IA     | Artifact that defines how AI can and cannot be used in the project.                              |
| Decision Journal            | Diario de decisiones                | Artifact used to record and review important decisions over time.                                |
| Product Backlog             | Backlog de producto                 | Ordered or grouped list of future work items, product hypotheses, requirements, or improvements. |

## Implementation Terms

| Term            | Spanish / Domain Equivalent | Definition                                                                                        |
| --------------- | --------------------------- | ------------------------------------------------------------------------------------------------- |
| Java            | Java                        | Main programming language for progressive implementation and executable validation.               |
| Spring Boot     | Spring Boot                 | Possible future Java framework for API/backend development.                                       |
| API             | API                         | Interface that allows software components or systems to communicate.                              |
| Backend         | Backend                     | Server-side part of an application that manages logic, data, or services when required.           |
| Database        | Base de datos               | Structured persistent storage mechanism that may be introduced when product behavior requires it. |
| Authentication  | Autenticación               | Process of verifying user identity.                                                               |
| Authorization   | Autorización                | Process of deciding what an authenticated user can access or do.                                  |
| Persistence     | Persistencia                | Ability to preserve data beyond temporary execution memory.                                       |
| In-Memory Data  | Datos en memoria            | Data kept temporarily while an application or executable experiment runs.                         |
| Production Code | Código de producción        | Code intended for real application use rather than only experimentation or learning validation.   |

## Open Terminology Questions

The following terms require future clarification when relevant to selected I2 behavior:

- Should the main actor remain `Caregiver`, or does selected behavior justify another actor distinction?
- Should `Bookmark Content` and `Save Content` mean the same thing?
- Should `Daily Tip` be modeled as a type of `Content Item`?
- Should `Resource` be a type of `Content Item` or a separate concept?
- Should `Audio Content` be independent content or an alternate representation of a content item?
- Does selected behavior require a `Profile`, authentication, or persistent user identity?
- Should Colombian child-rights terminology be researched and cited before adding authoritative user-facing content?

These questions should be refined only when they materially affect the selected use case, domain model, architecture, or implementation evidence.

## Glossary Maintenance Rules

This glossary should evolve when project evidence, decisions, or implementation materially change shared terminology.

Rules:

- New important terms should be added when they become relevant to requirements, analysis, design, architecture, code, or tests.
- Ambiguous terms should be clarified before they materially affect implementation.
- Product and domain terms may include Spanish equivalents.
- Technical terms should remain mainly in English.
- Terms should be updated when project decisions change.
- Prototype terminology should not automatically become implementation terminology.
- The glossary should remain lightweight and avoid defining concepts before they are needed.

## Current Glossary Position

This glossary establishes a shared vocabulary for KUNNA.

It connects the product domain, software engineering process, GitHub workflow, requirements, analysis, design, implementation, testing, and traceability.

The glossary originated during I1 and remains a living baseline during I2.

Terms should be expanded or refined only when they become materially relevant to the selected behavior and engineering evidence.
