# KUNNA Software Design

KUNNA is a personal software engineering project based on an original UX/UI prototype created several years ago. The original prototype was designed as a user experience and interface design project. This repository rebuilds that idea as a professional software engineering project.

The goal is not only to create an application, but to document the complete engineering process behind it: product vision, user goals, use cases, requirements, domain modeling, UML diagrams, object-oriented analysis, design decisions, Java implementation, and future API development with Spring Boot.

## Project Purpose

KUNNA is focused on mothers, fathers, and caregivers. Its product domain includes children's rights, positive parenting, daily tips, audio content, bookmarks, downloads, search, user profile, and content sharing.

The project is designed as professional portfolio evidence for software engineering learning and employability.

## Why This Project Exists

KUNNA started as a UX/UI prototype. However, this repository treats the product as a software engineering case study.

The purpose is to show how an initial product idea can be transformed into a structured software project through:

- Problem analysis.
- User goal definition.
- Use-case modeling.
- Supplementary requirements.
- Glossary and domain language.
- Risk identification.
- Iterative development planning.
- Architecture and design decisions.
- Object-oriented design.
- Progressive Java implementation.

## Strategic Approach

This project follows an iterative software engineering approach inspired by:

- Object-oriented analysis and design.
- UML modeling.
- Use-case driven development.
- Craig Larman's process-oriented approach from _Applying UML and Patterns_.
- Product-first thinking: problem, user outcome, decision-making, and implementation as a consequence.

The project also follows a product-first principle:

> Code is a means, not the goal.

This means implementation decisions should be justified by the problem, the users, the expected outcomes, and the design artifacts.

## Current Phase

The project is currently in:

**I1 — Inception Package**

The objective of this phase is to clarify the foundation of the project before writing production code.

This phase includes:

- Initial repository structure.
- Project vision.
- User goals.
- Initial use case model.
- Supplementary specification.
- Glossary.
- Risk list.
- Development plan.
- Development framework.
- AI collaboration policy.
- Decision journal.
- Product backlog.
- ADR-0001: Start with Inception Before Coding.

## Language Rule

Technical language: English.  
Product and domain language: Spanish.

This means:

- Repository documentation: mainly English.
- Code, commits, branches, issues, pull requests, and ADRs: mainly English.
- User-facing product content: Spanish.
- Colombian domain context: Spanish.
- README: English as the main language, with Spanish context when useful.

## Repository Structure

```text
kunna-software-design/
│
├── README.md
├── docs/
│   ├── 00-vision.md
│   ├── 01-user-goals.md
│   ├── 02-use-case-model.md
│   ├── 03-supplementary-specification.md
│   ├── 04-glossary.md
│   ├── 05-risk-list.md
│   ├── 06-development-plan.md
│   ├── 07-development-framework.md
│   ├── 08-ai-collaboration-policy.md
│   └── 09-decision-journal.md
│
├── research/
│   ├── original-ux-case-study.md
│   ├── competitive-landscape.md
│   └── prototype-notes.md
│
├── decisions/
│   └── ADR-0001-start-with-inception.md
│
├── backlog/
│   └── product-backlog.md
│
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── product-issue.md
    │   ├── technical-task.md
    │   └── decision-task.md
    └── pull_request_template.md
```

## Development Workflow

The project uses a professional GitHub-based workflow:

```
Issue → Branch → Artifact → Commit → Pull Request → Review → Merge → Done
```

Each relevant task should be connected to:

- A GitHub Issue.
- A milestone.
- A project board status.
- A clear commit message.
- A pull request when changes are integrated into main.

## Current Milestone

**I1 — Inception Package**

This milestone organizes the initial software engineering foundation for KUNNA.

The current focus is documentation, analysis, product reasoning, and project structure.

Production code is intentionally out of scope at this stage.

## Core Rules

- Do not start with production code.
- Do not add code that cannot be explained.
- Use documentation as engineering evidence.
- Document important decisions.
- Connect every major artifact to a GitHub Issue.
- Use AI as support, not as authority.
- Every concept learned should produce a concrete artifact in KUNNA.

## Professional Evidence

This repository is intended to demonstrate growth in:

- Software engineering fundamentals.
- GitHub project organization.
- Requirements analysis.
- Use-case driven development.
- UML and object-oriented modeling.
- Technical documentation.
- Decision-making.
- Java learning.
- Portfolio construction.

## Spanish Summary

KUNNA es un proyecto personal de ingeniería de software basado en un prototipo UX/UI original. El objetivo no es reconstruir únicamente una interfaz, sino convertir la idea en un proyecto profesional documentado, con visión de producto, usuarios, casos de uso, requisitos, decisiones, UML, diseño orientado a objetos e implementación progresiva en Java.

El proyecto se encuentra actualmente en la fase I1 — Inception Package, enfocada en entender el problema, definir el alcance inicial y preparar la base antes de escribir código de producción.
