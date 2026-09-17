# 06 — Development Plan

## Document Purpose

This document maintains the current development plan for KUNNA.

The plan was initially created during **I1 — Inception Package** and is now updated for **I2 — Elaboration**.

Its purpose is to describe the project's current phase, development direction, sequencing, and transition criteria without duplicating the detailed engineering practices defined in other artifacts.

Detailed execution rules are defined primarily in:

- `docs/05-risk-list.md`
- `docs/07-development-framework.md`
- `docs/08-ai-collaboration-policy.md`
- `docs/09-decision-journal.md`
- `backlog/product-backlog.md`

## Project Context

KUNNA is a personal software engineering project based on an original UX/UI prototype.

The prototype provides historical product context and candidate product ideas, but it is not treated as validated implementation scope or evidence of current user needs.

KUNNA is intended to demonstrate disciplined software engineering through:

- Product reasoning.
- Requirements analysis.
- Risk management.
- Use-case-driven development.
- Domain modeling.
- Object-oriented analysis and design.
- Selective UML.
- Architecture reasoning.
- Java implementation.
- Automated testing.
- Traceability.
- Professional Git and GitHub practices.
- Responsible AI-assisted collaboration.

Professional portfolio value should emerge from credible engineering evidence.

It must not determine product scope, architecture, technology selection, or artifact volume.

## Current Phase

The project is currently in:

**I2 — Elaboration**

The previous milestone, **I1 — Inception Package**, was completed and closed.

I2 focuses on reducing the most important product, requirements, domain, and architecture uncertainties around one architecturally significant use case.

The phase combines focused analysis with executable validation.

KUNNA will not attempt to complete the full product analysis or final architecture before implementation.

Instead, I2 will establish sufficient understanding around one selected slice, formulate an explicit architecture hypothesis, implement a small Java vertical slice with automated tests, and use the resulting evidence to reassess risks and future direction.

## Development Strategy

KUNNA follows a product-first, iterative, risk-driven, use-case-focused, and evidence-oriented development strategy.

Documentation and implementation are complementary engineering activities.

Documentation should be created or refined when it helps:

- Clarify product intent.
- Reduce current uncertainty.
- Define relevant behavior.
- Support an engineering decision.
- Prepare meaningful implementation.
- Preserve necessary traceability.

Implementation should begin when there is enough understanding to make the experiment meaningful, not when every possible analysis artifact is complete.

Implementation evidence may cause requirements, models, risks, backlog priorities, or architecture assumptions to change.

The project therefore follows these principles:

- Start from a product or engineering problem, not from a framework.
- Work around a focused use case rather than elaborating the complete system.
- Refine only requirements relevant to the current slice.
- Use modeling selectively.
- Treat architecture as a hypothesis until evidence supports it.
- Use Java implementation during Elaboration to reduce uncertainty.
- Use automated tests as evidence of meaningful behavior.
- Introduce infrastructure only when a demonstrated need justifies it.
- Preserve traceability from product intent to executable evidence.
- Keep portfolio concerns subordinate to product and engineering justification.

## Lifecycle Direction

KUNNA uses lightweight lifecycle phases inspired by iterative and Unified Process practices.

These phases are not rigid sequential stages.

Earlier artifacts may be refined when later evidence reveals new information.

| Phase                  | Status    | Main Purpose                                                                                                | Main Evidence                                                                                                             |
| ---------------------- | --------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| I1 — Inception Package | Completed | Establish the initial product and engineering baseline                                                      | Vision, goals, candidate use cases, supplementary requirements, risks, backlog, workflow, and initial decisions           |
| I2 — Elaboration       | Current   | Reduce significant product, domain, requirements, and architecture risks                                    | Selected use case, focused analysis, architecture hypothesis, Java vertical slice, automated tests, and risk reassessment |
| Construction           | Future    | Expand validated behavior incrementally                                                                     | Working product increments, tests, evolving design, and integration evidence                                              |
| Transition             | Future    | Prepare a sufficiently mature increment for realistic use, delivery, deployment, demonstration, or feedback | Deployable or demonstrable increment, known limitations, release information, and feedback                                |

Future phase names do not imply that corresponding GitHub milestones have already been approved.

A future milestone should be created only when the project has enough evidence to define its scope and exit criteria responsibly.

## I1 — Inception Package

### Status

**Completed**

I1 established the initial product and engineering baseline before deeper analysis and implementation.

Its principal artifacts include:

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
- `decisions/ADR-0001-start-with-inception.md`

I1 remains historical and closed.

Normal refinement caused by learning during I2 does not reopen the milestone.

## I2 — Elaboration

### Objective

Reduce the most significant current risks through one focused, traceable, and executable product slice.

I2 is not intended to:

- Complete every use case.
- Model the complete domain.
- Define every operation contract.
- Produce every possible UML diagram.
- Finalize the complete architecture.
- Build the complete product.
- Reconstruct every screen from the original prototype.
- Introduce infrastructure without demonstrated need.
- Produce production-ready software.

### Approved Work

The current milestone contains eight approved GitHub Issues:

1. **#29 — Review the I1 baseline and reprioritize key risks.**
2. **#30 — Select the architecturally significant use case for I2.**
3. **#31 — Refine the selected use case and relevant supplementary requirements.**
4. **#32 — Create a focused Domain Model and identify system operations.**
5. **#33 — Define the initial architecture hypothesis and validation strategy.**
6. **#34 — Build the first executable Java vertical slice with automated tests.**
7. **#35 — Evaluate the vertical slice and reassess architectural risks.**
8. **#36 — Assess I2 exit criteria and decide transition to Construction.**

Their current order reflects dependencies and risk reduction.

It does not define a one-way waterfall.

Evidence produced by later work may require earlier requirements, models, risks, backlog items, or architecture assumptions to be refined.

### Analysis Scope

Analysis should remain limited to what is necessary for the selected use case.

Depending on the problem and risk, I2 may use:

- Refined use case scenarios.
- Relevant supplementary requirements.
- Business rules.
- A focused Domain Model.
- System events and system operations.
- System Sequence Diagrams when useful.
- Operation contracts when additional state-change precision is necessary.
- GRASP or interaction reasoning when software responsibilities require clarification.

These techniques are selective.

Their detailed use is governed by `docs/07-development-framework.md`.

### Architecture and Executable Validation

Architecture during I2 should begin as an explicit hypothesis rather than as a presumed final structure.

The hypothesis should include only the decisions necessary to support the selected slice and reduce relevant risks.

It must be evaluated through a small executable Java vertical slice.

The slice should be:

- Focused on the selected use case.
- Small enough to understand and review.
- Traceable to relevant requirements and decisions.
- Executable.
- Automatically verified where meaningful.
- Sufficient to provide evidence about the architecture hypothesis.

The first slice is not required to be production-ready.

It may intentionally omit mechanisms such as:

- Web delivery.
- Persistence.
- Authentication.
- External services.
- Final UI.
- Deployment infrastructure.

Those mechanisms should be introduced only when the selected behavior or validation strategy demonstrates a concrete need.

### Evidence and Feedback

The intended I2 feedback path is:

```text
Selected use case
↓
Relevant requirements and business rules
↓
Focused domain analysis
↓
Architecture hypothesis
↓
Executable Java vertical slice
↓
Automated verification
↓
Observed evidence
↓
Risk and backlog reassessment
```

Implementation is therefore part of the learning process.

Evidence may cause previous assumptions or artifacts to change.

### I2 Exit Criteria

Completion of all eight Issues does not automatically justify transition to Construction.

Issue #36 must evaluate the evidence produced during Elaboration.

The project should have sufficient evidence that:

- The selected use case is understood well enough for incremental expansion.
- Relevant domain concepts are identified.
- Important system operations are understood.
- Relevant supplementary requirements are sufficiently clear.
- The architecture hypothesis has been exercised through executable Java behavior.
- Automated tests provide meaningful verification.
- Significant risks have been reduced, accepted, deferred, or explicitly carried forward.
- The backlog reflects current knowledge and evidence.
- Remaining uncertainty does not justify another focused Elaboration experiment before broader implementation.

If these conditions are not met, additional Elaboration work may be appropriate.

## Construction

Construction will expand software behavior incrementally from decisions that have already received some executable validation.

Construction does not mean that analysis, modeling, architecture, or risk management stop.

Future Construction work may include:

- Additional Java use case slices.
- Expanded domain behavior.
- Application coordination.
- Automated tests.
- Persistence when durable state is required.
- External services when justified.
- Delivery interfaces.
- Refactoring based on implementation evidence.
- Updated architecture decisions and documentation.

Construction should produce small, demonstrable increments rather than one large implementation effort.

## Technology Direction

Java remains the primary implementation language.

Spring Boot is not an approved mandatory phase or inevitable next technology.

An API is also not assumed to be required.

Spring Boot, REST interfaces, persistence, authentication, databases, external services, or similar infrastructure may be introduced only when a concrete product, integration, delivery, or architectural need justifies them.

Before adopting a significant technology, the project should be able to explain:

- What problem it solves.
- Which behavior requires it.
- Which risk it reduces or introduces.
- Whether a simpler alternative is sufficient.
- What additional complexity it creates.
- Whether the decision deserves an ADR.

Technology adoption should follow evidence rather than framework familiarity or portfolio expectations.

## Transition

Transition prepares a sufficiently mature increment for realistic use, delivery, deployment, demonstration, or feedback.

Possible work may include:

- Stabilization.
- Defect correction.
- Deployment validation.
- Usability and accessibility review.
- Security review appropriate to implemented scope.
- User or stakeholder feedback.
- Release information.
- Known limitations.
- Onboarding or usage instructions.
- Updated repository documentation.
- Demonstration material.
- Portfolio explanation.

Transition is therefore broader than portfolio preparation.

Portfolio communication should accurately represent the engineering work that actually occurred.

## Execution and Governance

The detailed execution workflow is defined by the Development Framework and the current backlog.

The current Project board workflow is:

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
Validation
↓
Merge
↓
Issue closure
```

For Markdown changes, the current quality controls include rendered Preview review and `git diff --check`.

The complete workflow should not be duplicated in this plan.

## Scope Control

To keep KUNNA realistic:

- Do not reopen I1 for normal I2 refinements.
- Do not elaborate the complete product before implementing the selected slice.
- Do not create UML diagrams or contracts mechanically.
- Do not treat prototype capabilities as validated requirements.
- Do not introduce infrastructure without demonstrated need.
- Do not design for hypothetical future scale without evidence.
- Do not allow portfolio value to override product or engineering reasoning.
- Do not treat repository organization as a substitute for executable evidence.
- Do not allow AI-assisted output to bypass human understanding and verification.
- Keep the current slice small enough to explain, test, review, and learn from.

## Historical I1 Work Order

The original Development Plan proposed the following Inception work order:

1. Repository structure.
2. README.
3. Project vision.
4. User goals.
5. Use case model.
6. Supplementary specification.
7. Glossary.
8. Risk list.
9. Development plan.
10. Development framework.
11. AI collaboration policy.
12. Decision journal.
13. Product backlog.
14. ADR-0001.

This list records the **original planned work order**, not necessarily the exact order in which all GitHub Issues were eventually completed.

It is retained only as historical context and does not define future phase sequencing.

## Portfolio Value

This development plan supports the professional value of KUNNA by making its evolution explainable.

Useful evidence includes:

- Product reasoning.
- Risk-driven prioritization.
- Selective analysis and modeling.
- Traceable decisions.
- Focused Git history.
- Pull requests.
- Java implementation.
- Automated tests.
- Architecture hypotheses and validation.
- Documented trade-offs.
- Evidence-based iteration.

Portfolio value should result from the engineering process that actually occurred rather than from maximizing the number of artifacts or technologies shown.

## Current Next Step

The current active work item is:

**GitHub Issue #29 — Review the I1 baseline and reprioritize key risks.**

This Development Plan is being updated because the previous version still described I1 as the active phase and separated Elaboration from the first executable Java evidence.

After Issue #29 is completed, Issue #30 may be prepared for execution:

**Select the architecturally significant use case for I2.**
