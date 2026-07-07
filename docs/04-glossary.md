# 04 — Glossary

## Document Purpose

This document defines the initial glossary for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to create a shared vocabulary for the project before moving into deeper analysis, design, UML modeling, and implementation.

A glossary helps reduce ambiguity across:

- Product vision.
- User goals.
- Use cases.
- Supplementary requirements.
- Domain modeling.
- Design decisions.
- Future Java implementation.

## Language Rule

KUNNA follows a hybrid language strategy:

- Technical language: English.
- Product and domain language: Spanish when useful.
- Repository artifacts: mainly English.
- User-facing content and Colombian domain examples: mainly Spanish.

This glossary may include both English and Spanish terms when that improves clarity.

## Core Product Terms

| Term                         | Spanish / Domain Equivalent        | Definition                                                                                                                                    |
| ---------------------------- | ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| KUNNA                        | KUNNA                              | Digital product designed to support caregivers with accessible content about children's rights, positive parenting, and daily care practices. |
| Product                      | Producto                           | The digital experience or system being designed and progressively implemented.                                                                |
| Prototype                    | Prototipo                          | The original UX/UI concept created in Figma, used as the starting point for the current software engineering project.                         |
| Software Engineering Project | Proyecto de ingeniería de software | The structured reconstruction of KUNNA through documentation, requirements, UML, design, decisions, and future implementation.                |
| Inception Package            | Paquete de Inicio                  | Initial set of artifacts that clarify the project vision, users, use cases, requirements, risks, plan, and decisions before coding.           |
| Product Vision               | Visión del producto                | High-level explanation of what KUNNA is, why it exists, who it serves, and what outcome it seeks.                                             |
| Product-First Approach       | Enfoque primero producto           | Strategy where the problem, users, and outcomes are clarified before implementation.                                                          |

## User and Actor Terms

| Term                  | Spanish / Domain Equivalent | Definition                                                                                                       |
| --------------------- | --------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| User                  | Usuario                     | Any person who interacts with KUNNA.                                                                             |
| Actor                 | Actor                       | A role that interacts with the system in a use case model.                                                       |
| Caregiver             | Cuidador / cuidadora        | Main user role. A person responsible for supporting, protecting, educating, or caring for a child in daily life. |
| Mother                | Madre                       | A caregiver role represented in the product domain.                                                              |
| Father                | Padre                       | A caregiver role represented in the product domain.                                                              |
| Guardian              | Acudiente / tutor           | A person legally or practically responsible for a child.                                                         |
| Guest User            | Usuario invitado            | A user who may access public content without authentication.                                                     |
| Registered Caregiver  | Cuidador registrado         | A caregiver with a profile, saved content, or preferences. This role is not fully defined yet.                   |
| Content Administrator | Administrador de contenido  | Possible future role responsible for creating, editing, or managing KUNNA content.                               |
| Primary Actor         | Actor primario              | The actor whose goal is fulfilled by a use case.                                                                 |
| Supporting Actor      | Actor de soporte            | An external system or role that helps complete a use case.                                                       |

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

| Term                | Spanish / Domain Equivalent    | Definition                                                                                                             |
| ------------------- | ------------------------------ | ---------------------------------------------------------------------------------------------------------------------- |
| Content             | Contenido                      | Any information item available in KUNNA, such as articles, tips, audio, resources, or child-rights explanations.       |
| Content Item        | Pieza de contenido             | A single unit of content that can be viewed, saved, shared, downloaded, or played if it has audio.                     |
| Daily Tip           | Tip diario                     | Short practical content that gives caregivers quick guidance.                                                          |
| Article             | Artículo                       | Longer content item that explains a topic in more detail.                                                              |
| Resource            | Recurso                        | Downloadable or reusable material that supports caregivers.                                                            |
| Audio Content       | Contenido en audio             | Content that can be listened to instead of read.                                                                       |
| Category            | Categoría                      | Grouping used to organize content by topic, such as child rights, positive parenting, daily care, resources, or audio. |
| Search Result       | Resultado de búsqueda          | A content item returned after the user searches for a topic or keyword.                                                |
| User-Facing Content | Contenido visible para usuario | Text, audio, labels, messages, or information shown directly to the caregiver.                                         |

## Interaction Terms

| Term                      | Spanish / Domain Equivalent          | Definition                                                                                            |
| ------------------------- | ------------------------------------ | ----------------------------------------------------------------------------------------------------- |
| View Content              | Ver contenido                        | Use case where a caregiver opens and reads or consults a content item.                                |
| View Daily Tip            | Ver tip diario                       | Use case where a caregiver accesses a short daily parenting or caregiving tip.                        |
| Browse Content Categories | Explorar categorías                  | Use case where a caregiver navigates available content by topic or category.                          |
| Search Content            | Buscar contenido                     | Use case where a caregiver searches for specific content using a keyword or topic.                    |
| Bookmark Content          | Guardar contenido / marcar contenido | Use case where a caregiver saves a content item for later consultation.                               |
| View Saved Content        | Ver contenido guardado               | Use case where a caregiver revisits previously saved content.                                         |
| Play Audio Content        | Reproducir audio                     | Use case where a caregiver listens to audio-based content.                                            |
| Download Resource         | Descargar recurso                    | Use case where a caregiver downloads a resource for later use.                                        |
| Share Content             | Compartir contenido                  | Use case where a caregiver shares a content item with another person or through an external platform. |
| Manage Profile            | Gestionar perfil                     | Use case where a registered caregiver manages profile information or preferences.                     |

## Requirements Terms

| Term                      | Spanish / Domain Equivalent | Definition                                                                                                               |
| ------------------------- | --------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Requirement               | Requisito                   | A condition or capability that the system should satisfy.                                                                |
| Functional Requirement    | Requisito funcional         | A requirement that describes what the system should do.                                                                  |
| Supplementary Requirement | Requisito complementario    | A requirement that applies across the system and is not fully described by one use case.                                 |
| Constraint                | Restricción                 | A limitation, rule, or condition that affects the project or solution.                                                   |
| Quality Attribute         | Atributo de calidad         | A characteristic of the system such as usability, accessibility, reliability, security, performance, or maintainability. |
| Usability                 | Usabilidad                  | How easy and understandable the product is for caregivers.                                                               |
| Accessibility             | Accesibilidad               | The degree to which the product can be used by people with different needs, abilities, or contexts.                      |
| Reliability               | Confiabilidad               | The ability of the system to behave consistently and predictably.                                                        |
| Security                  | Seguridad                   | Protection of data, access, and system behavior.                                                                         |
| Privacy                   | Privacidad                  | Responsible handling of user information and personal data.                                                              |
| Performance               | Rendimiento                 | How quickly the system responds or provides access to content.                                                           |
| Maintainability           | Mantenibilidad              | How easy it is to understand, modify, and improve the project over time.                                                 |
| Traceability              | Trazabilidad                | The ability to connect artifacts such as issues, commits, pull requests, requirements, and decisions.                    |

## Analysis and Design Terms

| Term                         | Spanish / Domain Equivalent         | Definition                                                                                                    |
| ---------------------------- | ----------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Use Case                     | Caso de uso                         | Description of how an actor interacts with the system to achieve a goal.                                      |
| Use Case Model               | Modelo de casos de uso              | Collection of actors, use cases, and relationships that describe system behavior from the user's perspective. |
| User Goal                    | Objetivo de usuario                 | What a user wants to accomplish with the product.                                                             |
| System Boundary              | Límite del sistema                  | The separation between what belongs inside KUNNA and what remains outside it.                                 |
| Domain Model                 | Modelo de dominio                   | Conceptual model that identifies important real-world concepts and relationships in the problem domain.       |
| UML                          | UML                                 | Unified Modeling Language, used to represent software analysis and design visually.                           |
| System Sequence Diagram      | Diagrama de secuencia del sistema   | Diagram that shows interactions between an actor and the system for a use case scenario.                      |
| Operation Contract           | Contrato de operación               | Description of what a system operation does, including preconditions and postconditions.                      |
| Object-Oriented Analysis     | Análisis orientado a objetos        | Process of understanding the problem domain using objects, concepts, responsibilities, and relationships.     |
| Object-Oriented Design       | Diseño orientado a objetos          | Process of assigning software responsibilities to objects and classes.                                        |
| GRASP                        | GRASP                               | Set of object-oriented design principles used to assign responsibilities to classes and objects.              |
| Architecture Decision Record | Registro de decisión arquitectónica | Document that records an important architecture or technical decision and its reasoning.                      |
| ADR                          | ADR                                 | Short form for Architecture Decision Record.                                                                  |

## GitHub Workflow Terms

| Term                | Spanish / Domain Equivalent | Definition                                                                                       |
| ------------------- | --------------------------- | ------------------------------------------------------------------------------------------------ |
| Repository          | Repositorio                 | GitHub project space that stores files, documentation, code, issues, pull requests, and history. |
| Issue               | Tarea / asunto              | Work item used to describe a task, problem, decision, requirement, or artifact to complete.      |
| Milestone           | Hito                        | Group of issues that belong to a specific project phase or goal.                                 |
| Project Board       | Tablero del proyecto        | Kanban-style board used to organize work by status.                                              |
| Backlog             | Pendiente                   | Work that has been identified but is not currently active.                                       |
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

| Term                        | Spanish / Domain Equivalent         | Definition                                                                             |
| --------------------------- | ----------------------------------- | -------------------------------------------------------------------------------------- |
| Artifact                    | Artefacto                           | A document, model, decision record, code file, or other project output.                |
| README                      | README                              | Main repository document that explains the project to visitors.                        |
| Vision Document             | Documento de visión                 | Artifact that defines the product idea, problem, users, scope, and outcomes.           |
| User Goals Document         | Documento de objetivos de usuario   | Artifact that identifies what users need to accomplish.                                |
| Use Case Model Document     | Documento de modelo de casos de uso | Artifact that identifies actors and candidate use cases.                               |
| Supplementary Specification | Especificación complementaria       | Artifact that documents cross-cutting requirements and constraints.                    |
| Glossary                    | Glosario                            | Artifact that defines project and domain terms.                                        |
| Risk List                   | Lista de riesgos                    | Artifact that identifies possible project risks.                                       |
| Development Plan            | Plan de desarrollo                  | Artifact that defines how the project will move forward.                               |
| Development Framework       | Marco de desarrollo                 | Artifact that defines process, workflow, and working rules.                            |
| AI Collaboration Policy     | Política de colaboración con IA     | Artifact that defines how AI can and cannot be used in the project.                    |
| Decision Journal            | Diario de decisiones                | Artifact used to record important decisions over time.                                 |
| Product Backlog             | Backlog de producto                 | Ordered or grouped list of future work items, features, requirements, or improvements. |

## Implementation Terms

| Term            | Spanish / Domain Equivalent | Definition                                                                             |
| --------------- | --------------------------- | -------------------------------------------------------------------------------------- |
| Java            | Java                        | Main programming language planned for progressive implementation.                      |
| Spring Boot     | Spring Boot                 | Possible future Java framework for API/backend development.                            |
| API             | API                         | Interface that allows software components or systems to communicate.                   |
| Backend         | Backend                     | Server-side part of an application that manages logic, data, and services.             |
| Database        | Base de datos               | Structured storage system for application data.                                        |
| Authentication  | Autenticación               | Process of verifying user identity.                                                    |
| Authorization   | Autorización                | Process of deciding what an authenticated user can access or do.                       |
| Persistence     | Persistencia                | Ability to save data beyond temporary memory.                                          |
| In-Memory Data  | Datos en memoria            | Data stored temporarily while the application runs.                                    |
| Production Code | Código de producción        | Code intended for real application use, not only documentation or learning simulation. |

## Open Terminology Questions

The following terms require future clarification:

- Should the main actor be called `Caregiver`, `User`, or `Registered Caregiver` in the first implementation?
- Should `Bookmark Content` and `Save Content` mean the same thing?
- Should `Daily Tip` be a type of `Content Item`?
- Should `Resource` be a type of `Content Item` or a separate concept?
- Should `Audio Content` be independent content or an attribute of a content item?
- Should `Profile` exist before authentication is implemented?
- Should Colombian child-rights terminology be researched and cited before adding real content?

## Glossary Maintenance Rules

This glossary should evolve as the project grows.

Rules:

- New important terms should be added when they appear in requirements, UML, design, or code.
- Ambiguous terms should be clarified before implementation.
- Product/domain terms may include Spanish equivalents.
- Technical terms should remain mainly in English.
- Terms should be updated when project decisions change.
- The glossary should support future domain modeling.

## Summary

This glossary establishes a shared vocabulary for KUNNA.

It helps connect the product domain, software engineering process, GitHub workflow, requirements, UML modeling, design decisions, and future Java implementation.

The glossary will continue to evolve as the project moves from Inception into deeper analysis, design, and construction.
