# KUNNA Software Design

KUNNA is a personal software engineering project based on an original UX/UI prototype created several years ago. The original prototype was designed as a user experience and interface design project. This repository evolves that idea into a professional software engineering case study.

The goal is not only to create an application, but to produce credible and traceable engineering evidence through product reasoning, requirements, use cases, risk management, selective modeling, object-oriented analysis and design, architecture decisions, Java implementation, automated testing, and iterative validation.

## Project Purpose

KUNNA is focused primarily on mothers, fathers, and caregivers.

The original prototype explored capabilities related to children's rights, positive parenting, daily tips, audio content, bookmarks, downloads, search, user profiles, and content sharing.

These capabilities are treated as **product hypotheses and candidate scope**, not as validated requirements or guaranteed implementation commitments.

The project also serves as professional software engineering evidence for learning and employability. Portfolio value should result from the engineering work that actually occurs rather than determine product scope, architecture, or technology choices.

## Why This Project Exists

KUNNA started as a UX/UI prototype. This repository treats that product concept as a software engineering case study.

The purpose is to show how an initial product idea can evolve through:

- Product and problem analysis.
- User goal definition.
- Use-case modeling.
- Supplementary requirements.
- Glossary and domain language.
- Risk identification and reassessment.
- Iterative development planning.
- Selective UML and object-oriented analysis.
- Architecture hypotheses and design decisions.
- Progressive Java implementation.
- Automated verification.
- Evidence-based refinement.

## Strategic Approach

KUNNA follows an iterative, risk-aware, use-case-driven, and product-oriented software engineering approach inspired by:

- Object-oriented analysis and design.
- UML modeling.
- Use-case-driven development.
- Selected practices from Craig Larman's _Applying UML and Patterns_.
- Product-first thinking.
- Risk-driven planning.
- Incremental implementation and feedback.

The project follows a product-first principle:

> Code is a means, not the goal.

Implementation decisions should be justified by the problem, expected user outcomes, current risks, relevant requirements, and engineering evidence.

Documentation and implementation are complementary activities.

The project does not require every possible artifact or model before producing executable feedback.

## Current Phase

The project is currently in:

**I2 — Elaboration**

The previous milestone, **I1 — Inception Package**, was completed and closed.

I1 established the initial product and engineering baseline, including:

- Repository structure.
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

I2 now focuses on reducing important product, requirements, domain, and architecture risks around one architecturally significant use case.

The current direction is to:

- Select one significant use case.
- Refine only the behavior and supplementary requirements relevant to that slice.
- Create focused domain and system-operation analysis.
- Formulate an architecture hypothesis.
- Implement a small executable Java vertical slice.
- Add meaningful automated tests.
- Evaluate the resulting evidence.
- Reassess risks, architecture assumptions, and backlog priorities.

Elaboration is therefore **not analysis-only**.

Executable evidence is deliberately produced before broader Construction work begins.

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

The files currently present in `research/` are placeholders. Their presence does not represent completed user research, competitive analysis, or product validation.

## Development Workflow

KUNNA uses a professional GitHub-based workflow.

The Project board uses:

```text
Backlog → Ready → In Progress → Review → Done
```

Meaningful work should remain traceable through:

```text
Issue
↓
Branch
↓
Focused commits
↓
Pull request
↓
Review and validation
↓
Merge
↓
Issue closure
```

The detailed operational workflow is maintained in:

- `docs/06-development-plan.md`
- `docs/07-development-framework.md`

## Current Milestone

**I2 — Elaboration**

The milestone contains the current sequence of risk-reduction work:

1. **#29 — Review the I1 baseline and reprioritize key risks.**
2. **#30 — Select the architecturally significant use case for I2.**
3. **#31 — Refine the selected use case and relevant supplementary requirements.**
4. **#32 — Create a focused Domain Model and identify system operations.**
5. **#33 — Define the initial architecture hypothesis and validation strategy.**
6. **#34 — Build the first executable Java vertical slice with automated tests.**
7. **#35 — Evaluate the vertical slice and reassess architectural risks.**
8. **#36 — Assess I2 exit criteria and decide transition to Construction.**

This sequence reflects current dependencies and risk reduction.

It is not a rigid waterfall. Implementation evidence may cause requirements, models, risks, architecture assumptions, or backlog priorities to be refined.

## Technology Direction

Java is the primary implementation language.

Spring Boot, REST APIs, persistence, databases, authentication, external services, or other infrastructure are **not predetermined requirements**.

They may be introduced when a concrete product, delivery, integration, or architecture need justifies them.

Technology choices should follow evidence rather than portfolio expectations.

## Core Rules

- Understand enough of the current product and engineering problem before implementing.
- Keep work focused on current value, risk, and evidence.
- Do not treat prototype capabilities as validated requirements.
- Use documentation and modeling selectively.
- Do not create UML artifacts only for completeness.
- Do not introduce frameworks or infrastructure without demonstrated need.
- Keep important decisions traceable.
- Connect meaningful work to GitHub Issues and pull requests.
- Use automated tests as evidence of implemented behavior.
- Use AI as support, not as authority.
- Preserve human understanding and responsibility for accepted work.
- Prefer credible engineering evidence over artifact or technology volume.

## Professional Evidence

This repository is intended to demonstrate growth in:

- Software engineering fundamentals.
- Product-oriented engineering.
- GitHub project organization.
- Requirements analysis.
- Risk management.
- Use-case-driven development.
- UML and object-oriented modeling.
- Architecture reasoning.
- Technical documentation.
- Decision-making.
- Java implementation.
- Automated testing.
- Traceability.
- Evidence-based iteration.

The professional value of KUNNA should come from the quality and explainability of the engineering process that actually occurred.

## Spanish Summary

KUNNA es un proyecto personal de ingeniería de software basado en un prototipo UX/UI original. El objetivo no es reconstruir únicamente una interfaz, sino evolucionar esa idea mediante análisis de producto, requisitos, gestión de riesgos, casos de uso, modelado selectivo, diseño orientado a objetos, decisiones de arquitectura, implementación progresiva en Java y pruebas automatizadas.

El proyecto se encuentra actualmente en **I2 — Elaboration**. Después de completar **I1 — Inception Package**, la prioridad es seleccionar un caso de uso arquitectónicamente significativo, refinar únicamente lo necesario para ese alcance, formular una hipótesis de arquitectura y validarla mediante una pequeña vertical slice ejecutable en Java con pruebas automatizadas.

Las capacidades del prototipo original se consideran hipótesis de producto hasta que exista evidencia suficiente para justificar su prioridad o implementación.
