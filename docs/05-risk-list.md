# 05 — Initial Risk List

## Document Purpose

This document defines the initial risk list for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to identify project, product, technical, documentation, and learning risks before moving into deeper analysis, modeling, design, and implementation.

This risk list helps keep the project realistic, focused, and useful as professional software engineering portfolio evidence.

## Context

KUNNA is a personal software engineering project based on an original UX/UI prototype.

The project aims to rebuild the concept as professional evidence of software engineering practice, including product thinking, requirements documentation, UML modeling, object-oriented analysis, design decisions, Java implementation, and future API development with Spring Boot.

Because this project has both a learning purpose and a portfolio purpose, the main risk is not only technical failure. The main risk is losing focus, overbuilding, overdocumenting, or creating artifacts that do not clearly support the product vision.

## Risk Evaluation Criteria

Each risk is described using the following criteria:

| Criterion   | Meaning                                          |
| ----------- | ------------------------------------------------ |
| Risk        | What could go wrong.                             |
| Area        | The part of the project affected by the risk.    |
| Impact      | How serious the risk would be if it happens.     |
| Probability | How likely the risk is at this stage.            |
| Mitigation  | What will be done to reduce or control the risk. |
| Status      | Current state of the risk.                       |

## Initial Risk List

| ID  | Risk                                                                                                                   | Area                  | Impact | Probability | Mitigation                                                                                                                                       | Status |
| --- | ---------------------------------------------------------------------------------------------------------------------- | --------------------- | ------ | ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------ |
| R01 | The project becomes too broad before the first useful version is defined.                                              | Product scope         | High   | Medium      | Keep the first version focused on a small set of core caregiver goals and candidate use cases.                                                   | Open   |
| R02 | The project becomes overdocumented before producing useful software behavior.                                          | Documentation         | Medium | Medium      | Use documentation selectively. Each artifact must support product vision, requirements, design, or implementation decisions.                     | Open   |
| R03 | The original UX/UI prototype influences the project too strongly without validating current user needs.                | Product validation    | High   | Medium      | Treat the prototype as a starting point, not as a fixed solution. Connect features to current user goals and use cases.                          | Open   |
| R04 | The project uses AI assistance without enough personal understanding from the project owner.                           | Learning process      | High   | Medium      | Every artifact must be reviewed, explained, and adapted by the project owner before being accepted.                                              | Open   |
| R05 | Technical implementation starts before the domain, use cases, and requirements are clear.                              | Engineering process   | High   | Medium      | Complete the Inception Package before moving into detailed design and Java implementation.                                                       | Open   |
| R06 | The project applies UML diagrams mechanically without improving analysis or design.                                    | UML modeling          | Medium | Medium      | Use UML only when it clarifies actors, use cases, domain concepts, relationships, responsibilities, or design decisions.                         | Open   |
| R07 | The language strategy becomes inconsistent between English technical documentation and Spanish product/domain content. | Documentation quality | Medium | Medium      | Keep technical artifacts mainly in English and product/domain examples in Spanish when useful.                                                   | Open   |
| R08 | The project tries to include advanced technologies too early, such as Spring Boot, APIs, authentication, or databases. | Technical scope       | High   | Medium      | Start with analysis, requirements, and simple Java/domain modeling before moving to framework-based implementation.                              | Open   |
| R09 | The product handles sensitive family, caregiver, or child-related topics without enough care.                          | Domain sensitivity    | High   | Medium      | Keep the first version educational and supportive. Avoid medical, legal, or psychological claims unless properly validated.                      | Open   |
| R10 | Requirements are written but not connected to use cases, decisions, or future implementation.                          | Traceability          | Medium | Medium      | Maintain links between vision, user goals, use cases, supplementary requirements, backlog items, and decisions.                                  | Open   |
| R11 | The backlog becomes a list of tasks instead of a prioritized product roadmap.                                          | Product management    | Medium | Medium      | Prioritize backlog items according to user value, learning value, and portfolio evidence value.                                                  | Open   |
| R12 | The repository looks organized but does not clearly communicate professional value to recruiters or reviewers.         | Portfolio value       | High   | Medium      | Keep the README, documentation structure, issues, pull requests, and commits clean, explainable, and connected to software engineering practice. | Open   |

## Priority Risks

At this stage, the most important risks are:

1. **R01 — Scope becomes too broad.**
2. **R04 — AI assistance without personal understanding.**
3. **R05 — Implementation starts too early.**
4. **R08 — Advanced technologies are introduced too soon.**
5. **R12 — The repository does not clearly communicate professional value.**

These risks are important because KUNNA is not only an application idea. It is also a software engineering learning and portfolio project.

## Risk Mitigation Strategy

The project will manage risk through an incremental workflow:

1. Complete the Inception Package before writing production code.
2. Keep each artifact connected to a GitHub issue and pull request.
3. Use branches for every meaningful change.
4. Use the project board to track progress.
5. Use milestones to measure package completion.
6. Avoid adding technologies before the design justifies them.
7. Review every AI-assisted artifact before accepting it.
8. Prefer clarity and traceability over large documents.

## Connection with Larman's Approach

This risk list supports an iterative and use-case-driven software engineering process inspired by Craig Larman's object-oriented analysis and design approach.

The project will not apply UML, operation contracts, or design patterns mechanically. Instead, these techniques will be used only when they help clarify the problem, the domain, the system behavior, or future implementation decisions.

This keeps the project aligned with a practical principle:

> Software engineering artifacts should improve understanding before implementation.

## Current Decision

The project will continue with documentation-first and product-first work during the Inception Package.

Implementation will start only after the core product direction, user goals, use cases, supplementary requirements, glossary, risks, development plan, collaboration policy, decision journal, and initial backlog are documented.

## Notes

This risk list is intentionally initial and will evolve as the project progresses.

New risks may be added during analysis, design, implementation, testing, or portfolio review.
