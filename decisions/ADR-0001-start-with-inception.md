# ADR-0001 — Start with Inception Before Coding

## Status

Accepted

## Decision Date

2026-07-01

## Last Reviewed

2026-08-02

## Context

KUNNA originated as a UX/UI prototype created several years ago.

The original prototype demonstrated the product concept, visual direction, and intended user experience. However, it did not document a complete software engineering process, domain model, architecture, implementation strategy, testing approach, or traceability between product decisions and technical work.

The current objective is not to reproduce the original interface immediately. The objective is to rebuild KUNNA as a professional software engineering project that demonstrates:

- Product thinking.
- Requirements analysis.
- Use-case-driven development.
- Supplementary requirements.
- Risk management.
- Domain modeling.
- Object-oriented analysis and design.
- Selective UML modeling.
- Architecture reasoning.
- Java implementation.
- Future API development with Spring Boot.
- Testing practices.
- Technical documentation.
- Professional Git and GitHub workflows.
- Responsible AI-assisted collaboration.
- Traceability between decisions, artifacts, and implementation.

Starting directly with production code would create several risks:

- Reproducing screens without validating the product purpose.
- Making implementation decisions before understanding the domain.
- Creating classes that mirror interface components instead of domain concepts.
- Losing traceability between user needs, requirements, use cases, and code.
- Overengineering the solution prematurely.
- Building functionality that does not clearly support the product vision.
- Producing weak portfolio evidence focused only on code output.
- Making architectural decisions without an explicit rationale.

KUNNA therefore requires a lightweight but explicit foundation before production implementation begins.

## Decision Drivers

The decision is guided by the following factors:

- The project must preserve the original product vision while allowing it to evolve.
- The primary users and their goals must be understood before implementation.
- Requirements and use cases must guide development.
- Sensitive family, childhood, and caregiving content requires deliberate product and privacy decisions.
- The project should demonstrate professional engineering reasoning, not only interface construction.
- UML and documentation should be used selectively and only when they provide design or communication value.
- Java implementation should emerge from validated product and domain understanding.
- Risks must be identified before irreversible technical decisions are made.
- The project must remain realistic for a personal learning and portfolio context.
- AI-assisted tools must support, rather than replace, human understanding and accountability.

## Decision

KUNNA will begin with a lightweight **Inception Package** before production code is written.

The Inception Package establishes the initial software engineering foundation of the project. It is not intended to produce exhaustive documentation or a complete upfront design.

Its purpose is to create enough shared understanding to begin iterative analysis, design, and implementation responsibly.

The first milestone is:

**I1 — Inception Package**

The milestone includes:

- Initial repository structure.
- Initial README.
- Initial project vision.
- Initial user goals.
- Initial use case model.
- Initial supplementary specification.
- Initial glossary.
- Initial risk list.
- Development plan.
- Development framework.
- Initial product backlog.
- AI collaboration policy.
- Decision journal.
- ADR-0001.

After the Inception Package is completed, the project may continue into deeper analysis, domain modeling, object-oriented design, architecture exploration, and incremental Java implementation.

## Inception Principles

The Inception Package will follow these principles:

### Lightweight

Artifacts must contain enough information to support decisions and future work, but they must not become exhaustive specifications.

### Product-Oriented

Every artifact must support the product vision, user goals, domain understanding, or implementation strategy.

### Iterative

The artifacts are initial versions. They may be refined as new information becomes available.

### Risk-Aware

Early work should reduce uncertainty around product scope, domain sensitivity, technical feasibility, architecture, and portfolio value.

### Use-Case-Driven

User goals and use cases will help guide requirements, modeling, design, implementation, and testing.

### Architecture-Aware

Architecture will be explored progressively. The project will not attempt to define a complete final architecture during inception.

### Traceable

Significant decisions and work items should be connected to relevant artifacts, issues, pull requests, risks, backlog items, or ADRs.

### Selective in Documentation

Documentation, UML, and formal analysis will be created only when they improve understanding, communication, design, validation, or traceability.

## Alternatives Considered

### Alternative 1 — Start Coding Immediately

Begin by recreating the original UX/UI prototype and adding functionality directly.

#### Advantages

- Produces visible results quickly.
- Creates an early executable application.
- Provides immediate Java or frontend practice.

#### Disadvantages

- Encourages implementation before product and domain understanding.
- May reproduce the old interface without validating current user needs.
- Creates a high risk of rework.
- Weakens traceability.
- May result in UI-driven classes instead of domain-oriented models.
- Provides limited evidence of engineering reasoning.

#### Outcome

Rejected.

### Alternative 2 — Complete a Full Upfront Design

Define all requirements, UML models, architecture, database structures, interfaces, and technical decisions before implementation.

#### Advantages

- Produces extensive documentation.
- Attempts to reduce uncertainty before coding.
- Creates a detailed initial plan.

#### Disadvantages

- Assumes knowledge that the project does not yet possess.
- Delays learning through implementation and validation.
- Encourages overdocumentation and speculative design.
- Conflicts with the iterative nature of the project.
- Is unrealistic for a personal learning and portfolio project.

#### Outcome

Rejected.

### Alternative 3 — Begin with a Lightweight Inception Package

Create the minimum engineering foundation needed to begin iterative development responsibly.

#### Advantages

- Connects product thinking with future implementation.
- Reduces major product and technical uncertainties.
- Creates explicit project traceability.
- Supports disciplined but incremental development.
- Preserves flexibility.
- Produces credible portfolio evidence.
- Aligns with use-case-driven and risk-aware engineering.

#### Disadvantages

- Delays production code temporarily.
- Requires disciplined documentation work.
- May create unnecessary overhead if artifacts are not kept lightweight.
- Requires periodic review to prevent documentation from becoming stale.

#### Outcome

Accepted.

## Consequences

### Positive Consequences

- KUNNA begins with a documented product and engineering foundation.
- User goals and use cases can guide later implementation.
- Risks are identified before major technical commitments.
- Architecture and domain modeling can emerge from explicit needs.
- GitHub issues, branches, commits, pull requests, and milestones become traceable engineering evidence.
- Future Java code will have clearer justification.
- The project demonstrates analysis, design, decision-making, and implementation skills.
- Documentation can support portfolio explanations and technical interviews.
- AI-assisted collaboration is governed from the beginning.

### Negative Consequences

- Production implementation begins later.
- The project requires maintaining several engineering artifacts.
- Some early assumptions may later prove incorrect.
- Documentation may become obsolete if it is not reviewed.
- There is a risk of overengineering or overdocumenting the project.

### Mitigations

To control the negative consequences:

- Documentation will remain lightweight and purpose-driven.
- Artifacts will be reviewed incrementally.
- UML will be used selectively.
- Decisions will include review triggers.
- The backlog will remain refinable.
- Production code will begin once the Inception Package provides sufficient clarity.
- New information may update artifacts without invalidating the entire process.
- Documentation work must remain connected to concrete product or engineering value.

## Relationship with Larman-Inspired Practices

This decision is influenced by the following software engineering ideas:

- Understand requirements before assigning software responsibilities.
- Use cases describe system behavior from the users' perspective.
- Domain concepts should be identified before creating implementation classes.
- Object-oriented design requires reasoning about responsibilities and collaborations.
- UML is a supporting communication tool, not the primary objective.
- Design artifacts should be created when they help answer relevant engineering questions.
- Development should remain iterative rather than attempting to complete all analysis and design upfront.

KUNNA does not adopt the Unified Process as a rigid methodology.

Instead, it selectively applies useful principles such as:

- Inception.
- Iterative development.
- Risk-driven planning.
- Use-case-driven analysis.
- Domain modeling.
- Object-oriented responsibility assignment.
- Selective UML.
- Progressive architecture and implementation.

## Implementation Guidance

After completing the Inception Package, the project should proceed incrementally through:

1. Product backlog refinement.
2. Selection of a small, valuable product slice.
3. Detailed use case refinement when necessary.
4. Domain modeling.
5. System operation identification.
6. Selective operation contracts when additional behavioral precision is useful.
7. Object-oriented analysis and responsibility assignment.
8. Architecture and design decisions.
9. Incremental Java implementation.
10. Automated and exploratory testing.
11. Review of risks, decisions, and documentation.
12. Preparation of the next iteration.

The sequence is not intended to be a strict waterfall. Activities may overlap and artifacts may evolve during implementation.

## Scope

This ADR governs the beginning of the KUNNA Software Design project.

It does not require:

- Complete requirements before implementation.
- Complete UML documentation.
- Complete architecture before coding.
- Final database design during inception.
- Full operation contracts for every use case.
- Production-ready deployment during the first milestone.
- Immediate recreation of every original prototype screen.

## Traceability

This decision is connected to:

- `README.md`
- `docs/00-vision.md`
- `docs/01-user-goals.md`
- `docs/02-use-case-model.md`
- `docs/03-supplementary-specification.md`
- `docs/04-glossary.md`
- `docs/05-risk-list.md`
- `docs/06-development-plan.md`
- `docs/07-development-framework.md`
- `docs/08-ai-collaboration-policy.md`
- `docs/09-decision-journal.md`
- `backlog/product-backlog.md`
- GitHub Milestone: `I1 — Inception Package`
- GitHub Issue: `#15`
- Decision Journal Entry: `DJ-001`

## Review Triggers

This ADR should be reviewed if:

- The Inception Package delays implementation without providing additional value.
- Documentation effort becomes greater than product or engineering progress.
- The product vision changes substantially.
- A new technical constraint invalidates the development approach.
- The project changes from a personal portfolio project to a production or team-based initiative.
- The selected lifecycle no longer supports iterative delivery.
- The project begins implementation without sufficient product or domain understanding.
- A future ADR supersedes the decision to begin with inception.

## Final Rationale

KUNNA will start with an Inception Package because the project aims to demonstrate professional software engineering practice rather than only reproduce a visual prototype.

The selected approach provides enough structure to understand the product, users, requirements, risks, development strategy, and decision process while preserving the flexibility required for iterative learning and implementation.

The intention is not to delay coding indefinitely.

The intention is to ensure that when implementation begins, it is connected to explicit product needs, domain understanding, engineering reasoning, and traceable decisions.
