# Product Backlog

## Document Purpose

This document defines the initial product backlog for KUNNA.

Its purpose is to translate the product vision, user goals, use cases,
supplementary requirements, risks, and development framework into
prioritized and actionable work items.

The backlog is not a fixed project plan. It is a living artifact that will
be reviewed and refined as the project gains new product and technical
knowledge.

## Current Milestone

**I1 — Inception Package**

The current milestone establishes the initial software engineering
foundation for KUNNA before deeper analysis, design, and production
implementation begin.

## Source Artifacts

The initial backlog is informed by:

- `README.md`
- `docs/00-vision.md`
- `docs/01-user-goals.md`
- `docs/02-use-case-model.md`
- `docs/03-supplementary-specification.md`
- `docs/04-glossary.md`
- `docs/05-risk-list.md`
- `docs/06-development-plan.md`
- `docs/07-development-framework.md`
- The original KUNNA UX/UI prototype.
- GitHub Issues and project board.

## Backlog Principles

The KUNNA backlog follows these principles:

- Product value comes before implementation volume.
- User goals guide feature selection.
- High-risk and high-uncertainty work is addressed early.
- Documentation must support a decision, deliverable, or learning outcome.
- UML is used selectively when it improves analysis, design, or communication.
- Production code is introduced only when the required foundation is clear.
- Backlog items should be small enough to understand, review, and complete.
- Every important implementation decision should be traceable to product
  needs, requirements, risks, or architecture decisions.
- AI-assisted work must remain reviewable and explainable by the project owner.

## Priority Model

| Priority        | Meaning                                                                |
| --------------- | ---------------------------------------------------------------------- |
| P0 — Foundation | Required before responsible implementation can begin.                  |
| P1 — MVP        | Required for the first valuable and demonstrable product increment.    |
| P2 — Important  | Valuable after the core MVP capabilities are stable.                   |
| P3 — Later      | Useful future capability that is not required for the initial product. |

## Status Model

| Status      | Meaning                                                                     |
| ----------- | --------------------------------------------------------------------------- |
| Backlog     | Identified but not prepared for immediate execution.                        |
| Ready       | Clear enough to begin and has no unresolved blocking dependency.            |
| In Progress | Currently being worked on.                                                  |
| Review      | Implementation or documentation is awaiting verification.                   |
| Done        | Acceptance criteria are satisfied and the result is integrated into `main`. |

## I1 — Inception Package Backlog

| ID           | GitHub Issue | Work Item                                          | Type                  | Priority | Status      |
| ------------ | -----------: | -------------------------------------------------- | --------------------- | -------- | ----------- |
| KUNNA-I1-001 |           #1 | Create initial repository structure                | Technical Task        | P0       | Done        |
| KUNNA-I1-002 |           #2 | Write initial README                               | Documentation         | P0       | Done        |
| KUNNA-I1-003 |           #3 | Write initial project vision                       | Product               | P0       | Done        |
| KUNNA-I1-004 |           #4 | Define user goals                                  | Requirements          | P0       | Done        |
| KUNNA-I1-005 |           #5 | Create initial use case model                      | Requirements          | P0       | Done        |
| KUNNA-I1-006 |           #6 | Write supplementary specification                  | Requirements          | P0       | Done        |
| KUNNA-I1-007 |           #7 | Create initial glossary                            | Documentation         | P0       | Done        |
| KUNNA-I1-008 |           #8 | Create initial risk list                           | Risk Management       | P0       | Done        |
| KUNNA-I1-009 |           #9 | Create development plan                            | Planning              | P0       | Done        |
| KUNNA-I1-010 |          #10 | Create development framework                       | Engineering           | P0       | Done        |
| KUNNA-I1-011 |          #11 | Create product backlog                             | Product Management    | P0       | In Progress |
| KUNNA-I1-012 |          #12 | Define AI collaboration policy                     | Governance            | P0       | Backlog     |
| KUNNA-I1-013 |          #13 | Create decision journal                            | Decision Management   | P0       | Backlog     |
| KUNNA-I1-014 |          #15 | Write ADR-0001: Start with inception before coding | Architecture Decision | P0       | Backlog     |

## Candidate Post-Inception Backlog

The following items are initial candidates for later iterations. They are not
commitments and may be split, reordered, rewritten, or removed during backlog
refinement.

### Product and Requirements

| ID           | Candidate Work Item                                        | Priority | Target Stage | Status  |
| ------------ | ---------------------------------------------------------- | -------- | ------------ | ------- |
| KUNNA-PB-001 | Define the first KUNNA MVP scope                           | P0       | Elaboration  | Backlog |
| KUNNA-PB-002 | Validate the primary caregiver journey                     | P0       | Elaboration  | Backlog |
| KUNNA-PB-003 | Refine the highest-value use cases                         | P0       | Elaboration  | Backlog |
| KUNNA-PB-004 | Define measurable outcomes for the first product increment | P0       | Elaboration  | Backlog |
| KUNNA-PB-005 | Review privacy and sensitive-content requirements          | P0       | Elaboration  | Backlog |

### Analysis and Modeling

| ID           | Candidate Work Item                                                 | Priority | Target Stage | Status  |
| ------------ | ------------------------------------------------------------------- | -------- | ------------ | ------- |
| KUNNA-PB-006 | Create the initial domain model                                     | P0       | Elaboration  | Backlog |
| KUNNA-PB-007 | Create system sequence diagrams for selected use cases              | P0       | Elaboration  | Backlog |
| KUNNA-PB-008 | Write operation contracts selectively for complex system operations | P1       | Elaboration  | Backlog |
| KUNNA-PB-009 | Refine supplementary requirements using quality scenarios           | P1       | Elaboration  | Backlog |
| KUNNA-PB-010 | Identify system responsibilities and conceptual boundaries          | P1       | Elaboration  | Backlog |

Operation contracts will be created only when a system operation requires
more analytical detail about preconditions, postconditions, object creation,
attribute changes, or associations. They will not be produced mechanically
for every operation.

### Architecture and Engineering

| ID           | Candidate Work Item                                               | Priority | Target Stage | Status  |
| ------------ | ----------------------------------------------------------------- | -------- | ------------ | ------- |
| KUNNA-PB-011 | Define the initial software architecture                          | P0       | Elaboration  | Backlog |
| KUNNA-PB-012 | Record significant architecture decisions with ADRs               | P0       | Elaboration  | Backlog |
| KUNNA-PB-013 | Define the initial Java project structure                         | P0       | Elaboration  | Backlog |
| KUNNA-PB-014 | Establish automated testing and quality checks                    | P0       | Elaboration  | Backlog |
| KUNNA-PB-015 | Implement the initial domain layer in Java                        | P1       | Construction | Backlog |
| KUNNA-PB-016 | Define persistence boundaries without premature database coupling | P1       | Construction | Backlog |
| KUNNA-PB-017 | Prepare the future Spring Boot API boundary                       | P2       | Construction | Backlog |

### Initial Product Capabilities

| ID           | Candidate Work Item                                     | Priority | Target Stage | Status  |
| ------------ | ------------------------------------------------------- | -------- | ------------ | ------- |
| KUNNA-PB-018 | Browse children's rights and positive-parenting content | P1       | Construction | Backlog |
| KUNNA-PB-019 | Search and filter available content                     | P1       | Construction | Backlog |
| KUNNA-PB-020 | View the details of a selected content item             | P1       | Construction | Backlog |
| KUNNA-PB-021 | Bookmark useful content                                 | P1       | Construction | Backlog |
| KUNNA-PB-022 | Listen to an audio version of supported content         | P1       | Construction | Backlog |
| KUNNA-PB-023 | Download supported content for later access             | P2       | Construction | Backlog |
| KUNNA-PB-024 | Share selected content through supported channels       | P2       | Construction | Backlog |
| KUNNA-PB-025 | Manage a basic caregiver profile                        | P2       | Construction | Backlog |
| KUNNA-PB-026 | Present daily parenting tips                            | P2       | Construction | Backlog |
| KUNNA-PB-027 | Explore responsible personalization options             | P3       | Future       | Backlog |

## Definition of Ready

A backlog item may move to `Ready` when:

- Its purpose and expected outcome are understandable.
- The relevant user, stakeholder, or engineering concern is identified.
- Major dependencies are known.
- Important risks or open questions are visible.
- The item is small enough to complete within a reasonable iteration.
- Acceptance criteria can be written.
- The project owner can explain why the item is valuable.

## Definition of Done

A backlog item may move to `Done` when:

- Its acceptance criteria are satisfied.
- The result has been reviewed.
- Relevant tests or verification activities have been completed.
- Documentation and traceability are updated when necessary.
- The change is committed with a clear Conventional Commit message.
- A pull request has been completed.
- The result is integrated into `main`.
- The project owner can explain the result and the decisions behind it.

## Backlog Refinement Rules

During refinement:

1. Review product value and user relevance.
2. Review risks, dependencies, and uncertainty.
3. Split work items that are too broad.
4. Remove items that no longer support the product vision.
5. Update priorities when new evidence appears.
6. Connect implementation work to requirements, use cases, or decisions.
7. Avoid introducing functionality only because it is technically interesting.
8. Keep GitHub Issues and this document reasonably synchronized.

## Current Next Steps

To complete the I1 — Inception Package:

1. Complete this initial product backlog.
2. Define the AI collaboration policy.
3. Create the decision journal.
4. Write ADR-0001: Start with inception before coding.

After those items are completed, the project may begin backlog refinement for
the first Elaboration iteration.
