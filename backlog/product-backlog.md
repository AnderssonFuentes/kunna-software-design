# Product Backlog

## Document Purpose

This document maintains the current product and engineering backlog for KUNNA.

Its purpose is to translate the product vision, user goals, use cases, supplementary requirements, risks, decisions, and current engineering evidence into prioritized and actionable work.

The backlog is not a fixed project plan.

It is a living artifact that may be refined, reordered, split, deferred, replaced, or removed as the project gains new product and technical knowledge.

## Current Milestone

**I2 — Elaboration**

I1 established the initial KUNNA engineering baseline and is now closed.

I2 focuses on reducing the most important product, domain, requirements, and architecture uncertainties around one architecturally significant use case.

The phase will combine focused analysis with executable validation rather than postponing all implementation until Construction.

The expected progression is:

```text
Review I1 baseline and risks
↓
Select an architecturally significant use case
↓
Refine only the relevant behavior and requirements
↓
Create a focused Domain Model and identify system operations
↓
Define an architecture hypothesis and validation strategy
↓
Build a small executable Java vertical slice with automated tests
↓
Evaluate evidence and reassess risks
↓
Decide whether transition toward Construction is justified
```

## Source Artifacts

The backlog is informed by:

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
- `decisions/ADR-0001-start-with-inception.md`
- GitHub Issues.
- GitHub Projects.
- GitHub Pull Requests.
- The original KUNNA UX/UI prototype.

The prototype is a source of product hypotheses, not proof of current user needs.

The current files under `research/` were created as placeholders during the initial workspace setup and do not yet provide user-validation or competitive-research evidence.

## Backlog Principles

The KUNNA backlog follows these principles:

- Product value comes before implementation volume.
- User goals and use cases guide product behavior.
- High-risk and high-uncertainty work should be addressed early.
- Current evidence and explicit assumptions should influence prioritization.
- Documentation and modeling should support a concrete decision, risk reduction, implementation need, or learning result.
- UML is used selectively when it improves analysis, design, validation, or communication.
- Implementation may be used during Elaboration to test assumptions and architecture hypotheses.
- Frameworks, persistence, authentication, APIs, databases, and other infrastructure are introduced only when a demonstrated need justifies them.
- Backlog items should be small enough to understand, review, and complete.
- Important implementation work should remain traceable to product intent, requirements, risks, or decisions.
- Learning value may influence sequencing, but portfolio value must not override product or engineering justification.
- AI-assisted work must remain reviewable, verifiable, and explainable by the project owner.

## Priority Model

Priority represents the current importance of a backlog item based on product value, risk reduction, uncertainty, dependency, and available evidence.

| Priority            | Meaning                                                                                               |
| ------------------- | ----------------------------------------------------------------------------------------------------- |
| P0 — Critical       | Required to unblock or complete the current milestone.                                                |
| P1 — High           | Important product or engineering work supported by current evidence or risk.                          |
| P2 — Medium         | Valuable work that does not currently drive the milestone.                                            |
| P3 — Later          | Candidate work that should remain deferred until stronger justification exists.                       |
| TBD — Unprioritized | Candidate work that has not yet received sufficient evaluation or evidence for a meaningful priority. |

Priority does not represent portfolio attractiveness or technical complexity alone.

## Status Model

| Status      | Meaning                                                                     |
| ----------- | --------------------------------------------------------------------------- |
| Backlog     | Identified but not prepared for immediate execution.                        |
| Ready       | Clear enough to begin and has no unresolved blocking dependency.            |
| In Progress | Currently being worked on.                                                  |
| Review      | The result is awaiting final verification or merge.                         |
| Done        | Acceptance criteria are satisfied and the result is integrated into `main`. |

## I1 — Inception Package History

I1 is complete.

The following table is retained as historical traceability and must not be interpreted as the current work queue.

The historical I1 priority values retain their original meaning from the Inception backlog. In that context, `P0` meant `Foundation` and should not be reinterpreted using the current I2 priority model.

| ID           | GitHub Issue | Work Item                                          | Type                  | Priority | Status |
| ------------ | -----------: | -------------------------------------------------- | --------------------- | -------- | ------ |
| KUNNA-I1-001 |           #1 | Create initial repository structure                | Technical Task        | P0       | Done   |
| KUNNA-I1-002 |           #2 | Write initial README                               | Documentation         | P0       | Done   |
| KUNNA-I1-003 |           #3 | Write initial project vision                       | Product               | P0       | Done   |
| KUNNA-I1-004 |           #4 | Define user goals                                  | Requirements          | P0       | Done   |
| KUNNA-I1-005 |           #5 | Create initial use case model                      | Requirements          | P0       | Done   |
| KUNNA-I1-006 |           #6 | Write supplementary specification                  | Requirements          | P0       | Done   |
| KUNNA-I1-007 |           #7 | Create initial glossary                            | Documentation         | P0       | Done   |
| KUNNA-I1-008 |           #8 | Create initial risk list                           | Risk Management       | P0       | Done   |
| KUNNA-I1-009 |           #9 | Create development plan                            | Planning              | P0       | Done   |
| KUNNA-I1-010 |          #10 | Create development framework                       | Engineering           | P0       | Done   |
| KUNNA-I1-011 |          #11 | Create product backlog                             | Product Management    | P0       | Done   |
| KUNNA-I1-012 |          #12 | Define AI collaboration policy                     | Governance            | P0       | Done   |
| KUNNA-I1-013 |          #13 | Create decision journal                            | Decision Management   | P0       | Done   |
| KUNNA-I1-014 |          #15 | Write ADR-0001: Start with inception before coding | Architecture Decision | P0       | Done   |

`KUNNA-I1-014` is the internal identifier for the fourteenth I1 backlog item.

It does not renumber GitHub Issues. I1 contains GitHub Issues `#1–#13` and `#15`; GitHub Issue `#14` is not part of the completed I1 milestone.

## I2 — Elaboration Backlog

The following eight GitHub Issues define the currently approved I2 work.

Their order reflects dependencies and risk reduction rather than a rigid waterfall. Evidence produced by later work may refine earlier artifacts when necessary.

| Order | GitHub Issue | Work Item                                                            | Primary Outcome                                                                                 | Main Risk Drivers            | Status      |
| ----: | -----------: | -------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ---------------------------- | ----------- |
|     1 |          #29 | Review the I1 baseline and reprioritize key risks                    | Reliable and current baseline for I2                                                            | R01, R02, R03, R08, R10, R11 | In Progress |
|     2 |          #30 | Select the architecturally significant use case for I2               | One explicitly justified use case selected for Elaboration                                      | R01, R03, R09, R11           | Backlog     |
|     3 |          #31 | Refine the selected use case and relevant supplementary requirements | Sufficient behavioral and quality detail for the selected slice                                 | R05, R09, R14, R15           | Backlog     |
|     4 |          #32 | Create a focused Domain Model and identify system operations         | Relevant domain concepts and system operations identified without modeling the complete product | R05, R06, R10                | Backlog     |
|     5 |          #33 | Define the initial architecture hypothesis and validation strategy   | Explicit architecture hypothesis and evidence plan                                              | R08, R10, R13, R15           | Backlog     |
|     6 |          #34 | Build the first executable Java vertical slice with automated tests  | Executable evidence for the selected behavior and architecture hypothesis                       | R04, R05, R08, R10, R13, R15 | Backlog     |
|     7 |          #35 | Evaluate the vertical slice and reassess architectural risks         | Observed results, lessons, and updated risk assessment                                          | R10, R13, R15                | Backlog     |
|     8 |          #36 | Assess I2 exit criteria and decide transition to Construction        | Explicit decision on whether the project is ready to expand implementation                      | R01, R08, R10, R11, R13      | Backlog     |

Only one I2 item should normally be `In Progress` when its predecessor still produces information required by the next item.

Items may move to `Ready` when their dependencies and acceptance criteria are sufficiently clear.

## Alignment of Existing Post-I1 Candidates

The initial backlog contained several broad post-Inception candidates.

They are retained below for traceability but are now mapped to the approved I2 workflow or explicitly deferred.

### Product and Requirements Candidates

| ID           | Original Candidate                                         | Current Treatment                                                                            | Related I2 Work                     |
| ------------ | ---------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------- |
| KUNNA-PB-001 | Define the first KUNNA MVP scope                           | Deferred. Defining the complete MVP is not required before the first Elaboration experiment. | Future refinement after I2 evidence |
| KUNNA-PB-002 | Validate the primary caregiver journey                     | Remains a product-research candidate. No current validation evidence is documented.          | Future research work                |
| KUNNA-PB-003 | Refine the highest-value use cases                         | Replaced by selecting and refining one significant use case.                                 | #30, #31                            |
| KUNNA-PB-004 | Define measurable outcomes for the first product increment | Partially incorporated into slice refinement and validation.                                 | #31, #35                            |
| KUNNA-PB-005 | Review privacy and sensitive-content requirements          | Apply selectively when relevant to the selected use case.                                    | #31; R09, R14                       |

### Analysis and Modeling Candidates

| ID           | Original Candidate                                                  | Current Treatment                                                                         | Related I2 Work |
| ------------ | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | --------------- |
| KUNNA-PB-006 | Create the initial domain model                                     | Replaced by a focused Domain Model for the selected slice.                                | #32             |
| KUNNA-PB-007 | Create system sequence diagrams for selected use cases              | Conditional. Create an SSD only when it improves understanding of system events.          | #32             |
| KUNNA-PB-008 | Write operation contracts selectively for complex system operations | Remains conditional and selective.                                                        | #32             |
| KUNNA-PB-009 | Refine supplementary requirements using quality scenarios           | Refine only requirements that materially affect the selected slice.                       | #31; R15        |
| KUNNA-PB-010 | Identify system responsibilities and conceptual boundaries          | Split across domain analysis and later software responsibility or architecture reasoning. | #32, #33        |

### Architecture and Engineering Candidates

| ID           | Original Candidate                                                | Current Treatment                                                                                                             | Related I2 Work                   |
| ------------ | ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------- |
| KUNNA-PB-011 | Define the initial software architecture                          | Reframed as an architecture hypothesis that must be validated through executable evidence.                                    | #33, #34, #35                     |
| KUNNA-PB-012 | Record significant architecture decisions with ADRs               | Conditional. Create an ADR only when a decision has sufficient architectural significance and durability.                     | #33 or later                      |
| KUNNA-PB-013 | Define the initial Java project structure                         | Replaced by the minimum project structure justified by the architecture hypothesis and vertical slice.                        | #34                               |
| KUNNA-PB-014 | Establish automated testing and quality checks                    | Incorporated into the first executable vertical slice.                                                                        | #34                               |
| KUNNA-PB-015 | Implement the initial domain layer in Java                        | Replaced by domain behavior implemented as part of the I2 vertical slice rather than postponed automatically to Construction. | #34                               |
| KUNNA-PB-016 | Define persistence boundaries without premature database coupling | Deferred unless the selected use case demonstrates a persistence need.                                                        | Future or conditional I2 work     |
| KUNNA-PB-017 | Prepare the future Spring Boot API boundary                       | Deferred. No API or Spring Boot adoption is currently approved.                                                               | Future decision only if justified |

## Candidate Product Capabilities

The following capabilities originate from the initial product concept, user-goal discussions, use case model, or original prototype.

They are **candidates, not commitments**.

Their previous P1–P3 assignments are not treated as validated product priorities because sufficient evidence and explicit prioritization rationale do not yet exist.

Issue `#30` will evaluate a limited set of use cases and select one architecturally significant flow for I2.

| ID           | Candidate Capability                                    | Priority | Evidence Status    | Status  |
| ------------ | ------------------------------------------------------- | -------- | ------------------ | ------- |
| KUNNA-PB-018 | Browse children's rights and positive-parenting content | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-019 | Search and filter available content                     | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-020 | View the details of a selected content item             | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-021 | Bookmark useful content                                 | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-022 | Listen to an audio version of supported content         | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-023 | Download supported content for later access             | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-024 | Share selected content through supported channels       | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-025 | Manage a basic caregiver profile                        | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-026 | Present daily parenting tips                            | TBD      | Product hypothesis | Backlog |
| KUNNA-PB-027 | Explore responsible personalization options             | TBD      | Product hypothesis | Backlog |

A candidate capability should not receive a product priority merely because it existed in the original prototype or appears technically interesting.

Its priority should be established from product value, risk, uncertainty, dependencies, and available evidence.

## Definition of Ready

A backlog item may move to `Ready` when:

- Its purpose and expected outcome are understandable.
- The relevant user, product, risk, or engineering concern is identified.
- Important assumptions are visible.
- Major dependencies are known.
- Blocking questions have been resolved sufficiently to begin.
- The item is small enough to complete within a focused iteration.
- Acceptance criteria can be evaluated.
- The project owner can explain why the work should happen now.

`Ready` does not require every uncertainty to be eliminated.

It requires enough clarity for the work to produce meaningful evidence or value.

## Definition of Done

A backlog item may move to `Done` when:

- Its acceptance criteria are satisfied.
- The result has been reviewed.
- Relevant tests or verification activities have been completed when applicable.
- Documentation and traceability are updated when necessary.
- The change is committed through focused history.
- A pull request has been completed.
- The result is integrated into `main`.
- The related GitHub Issue is closed.
- The project board reflects the final status.
- The project owner understands and can explain the result and its decisions.

## Backlog Refinement Rules

During refinement:

1. Review product value and user relevance.
2. Review current risks, uncertainty, dependencies, and evidence.
3. Distinguish validated information from assumptions or hypotheses.
4. Split work items that are too broad.
5. Reframe artifact-oriented tasks around the problem or uncertainty they address.
6. Remove or defer work that no longer supports the product direction.
7. Update priorities when new evidence appears.
8. Connect implementation work to relevant requirements, use cases, risks, or decisions.
9. Avoid introducing functionality or technology only because it is technically interesting or useful for portfolio appearance.
10. Keep GitHub Issues, the Project board, and this document reasonably synchronized without duplicating unnecessary operational detail.

## Current Next Step

The current active work item is:

**GitHub Issue #29 — Review the I1 baseline and reprioritize key risks.**

Issue #29 must establish a reliable I2 baseline before the project selects its architecturally significant use case.

After Issue #29 is completed, Issue #30 may move from `Backlog` to `Ready` and then to `In Progress` when its dependencies and acceptance criteria are confirmed.

The closed **I1 — Inception Package** milestone remains historical and is not reopened by normal I2 refinement.
