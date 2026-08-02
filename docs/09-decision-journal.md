# 09 — Decision Journal

## Document Purpose

This document defines the initial decision journal for KUNNA as part of
the **I1 — Inception Package**.

The purpose of this journal is to maintain a lightweight, chronological,
and traceable record of meaningful decisions made throughout the project.

The journal supports:

- Product reasoning.
- Requirements decisions.
- Process decisions.
- Modeling decisions.
- Architecture decisions.
- Implementation decisions.
- Testing and quality decisions.
- Responsible AI collaboration.
- Portfolio transparency.

The decision journal helps explain not only what was produced, but also
why important choices were made.

## Relationship with Other Artifacts

This journal complements the following project artifacts:

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
- `backlog/product-backlog.md`
- `decisions/ADR-0001-start-with-inception.md`

These documents contain the detailed product and engineering information.

The decision journal provides a concise record of the choices that connect
those artifacts.

## Decision Journal and ADRs

The decision journal and Architecture Decision Records serve related but
different purposes.

### Decision Journal

The decision journal records meaningful project decisions in a concise and
chronological format.

It may include decisions related to:

- Product direction.
- Requirements.
- Project workflow.
- Documentation.
- UML and modeling.
- Architecture.
- Technology.
- Testing.
- AI-assisted work.

### Architecture Decision Record

An Architecture Decision Record, or ADR, provides a more detailed analysis
of a decision with significant or long-term consequences.

An ADR normally documents:

- Context.
- Decision drivers.
- Considered alternatives.
- Final decision.
- Consequences.
- Trade-offs.

Not every journal entry requires an ADR.

An ADR should be created when a decision:

- Has significant architectural consequences.
- Is difficult or costly to reverse.
- Affects several parts of the system.
- Requires explicit comparison of alternatives.
- Is important enough to justify a permanent standalone record.

## What Should Be Recorded

A decision should be included in this journal when it affects one or more
of the following:

- Product scope.
- User value.
- Requirements interpretation.
- Development lifecycle.
- Documentation strategy.
- Modeling approach.
- Architecture.
- Technology selection.
- Testing strategy.
- Security or privacy.
- Repository workflow.
- AI collaboration.
- Portfolio representation.

Routine actions do not need individual decision entries.

Examples of routine actions that normally do not require entries include:

- Fixing formatting.
- Correcting spelling.
- Renaming a local variable.
- Deleting a merged branch.
- Updating a status after completing an issue.

## Decision Categories

KUNNA uses the following decision categories:

| Category       | Description                                                        |
| -------------- | ------------------------------------------------------------------ |
| Product        | Product purpose, users, scope, and value decisions                 |
| Requirements   | Functional and supplementary requirement decisions                 |
| Process        | Lifecycle, workflow, and documentation decisions                   |
| Modeling       | Use case, domain, UML, and object-oriented modeling decisions      |
| Architecture   | Structural and high-impact technical decisions                     |
| Implementation | Programming language, frameworks, and coding decisions             |
| Quality        | Testing, validation, security, privacy, and quality decisions      |
| AI Governance  | Responsible use of AI-assisted tools                               |
| Portfolio      | Decisions affecting professional evidence and project presentation |

## Decision Status

Each decision uses one of the following statuses:

| Status     | Meaning                                                             |
| ---------- | ------------------------------------------------------------------- |
| Proposed   | The decision is being considered                                    |
| Accepted   | The decision has been approved and currently applies                |
| Deferred   | The decision has been postponed until more information is available |
| Rejected   | The option was considered but not selected                          |
| Superseded | A newer decision has replaced the previous decision                 |

## Decision Entry Structure

Each journal entry should contain:

- Decision identifier.
- Date.
- Status.
- Category.
- Context.
- Decision.
- Rationale.
- Consequences.
- Related artifacts.
- Related ADR, when applicable.
- Review trigger.

The following template should be used for future entries:

```text
### DJ-XXX — Decision Title

**Date:** YYYY-MM-DD
**Status:** Proposed | Accepted | Deferred | Rejected | Superseded
**Category:** Product | Requirements | Process | Modeling | Architecture |
Implementation | Quality | AI Governance | Portfolio

#### Context

What situation, uncertainty, or problem required a decision?

#### Decision

What was decided?

#### Rationale

Why was this option selected?

#### Consequences

What positive, negative, or neutral consequences follow from the decision?

#### Related Artifacts

- Relevant file, issue, pull request, or milestone.

#### Related ADR

- ADR reference, or `Not required`.

#### Review Trigger

What future event or new information should cause this decision to be reviewed?
```

## Initial Decision Register

| ID     | Decision                                                                        | Category       | Status   | ADR                        |
| ------ | ------------------------------------------------------------------------------- | -------------- | -------- | -------------------------- |
| DJ-001 | Begin with an Inception Package before production code                          | Process        | Accepted | ADR-0001                   |
| DJ-002 | Use a hybrid English and Spanish language strategy                              | Process        | Accepted | Not required               |
| DJ-003 | Follow a product-oriented and iterative engineering approach                    | Product        | Accepted | Not required               |
| DJ-004 | Use UML selectively as a design and communication tool                          | Modeling       | Accepted | Not required               |
| DJ-005 | Use Java as the primary implementation language and introduce Spring Boot later | Implementation | Accepted | Future ADR may be required |
| DJ-006 | Use an issue, branch, pull request, merge, and cleanup workflow                 | Process        | Accepted | Not required               |
| DJ-007 | Use AI as a support tool while preserving human responsibility                  | AI Governance  | Accepted | Not required               |

---

## DJ-001 — Begin with an Inception Package Before Production Code

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Process

### Context

KUNNA began as an original UX/UI prototype created before the current
software engineering project.

The project could have moved directly into Java implementation. However,
doing so would have introduced production code before clarifying the product
vision, user goals, use cases, supplementary requirements, risks, workflow,
and engineering direction.

### Decision

KUNNA will begin with an initial Inception Package before production
implementation.

The package includes:

- Repository structure.
- Initial README.
- Product vision.
- User goals.
- Initial use case model.
- Supplementary specification.
- Glossary.
- Initial risk list.
- Development plan.
- Development framework.
- Product backlog.
- AI collaboration policy.
- Decision journal.
- ADR-0001.

### Rationale

The Inception Package establishes enough shared understanding to begin
deeper analysis and implementation with reduced ambiguity.

The intention is not to complete all possible documentation before coding.

The intention is to create a sufficient and traceable foundation for
iterative development.

### Consequences

Positive consequences:

- Product and engineering intent become explicit.
- Future implementation decisions can be traced to project artifacts.
- Premature coding and avoidable rework are reduced.
- The repository provides stronger professional portfolio evidence.

Potential negative consequences:

- Initial implementation begins later.
- Documentation could become excessive if it is not kept selective.
- Some early assumptions may change after validation.

### Related Artifacts

- `README.md`
- `docs/00-vision.md`
- `docs/06-development-plan.md`
- `docs/07-development-framework.md`
- GitHub milestone `I1 — Inception Package`
- GitHub Issue #15

### Related ADR

- `decisions/ADR-0001-start-with-inception.md`

### Review Trigger

Review this decision when the Inception Package is completed or when
documentation begins to delay useful product validation without reducing
meaningful risk.

---

## DJ-002 — Use a Hybrid English and Spanish Language Strategy

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Process

### Context

KUNNA is connected to a Colombian product and family-care context, while the
repository is also intended to demonstrate professional software engineering
practice.

Technical documentation and software development terminology are commonly
written in English, while user-facing content and domain examples may be
clearer and more appropriate in Spanish.

### Decision

KUNNA will use a hybrid language strategy:

- Technical language: English.
- Repository documentation: mainly English.
- Code, commits, branches, issues, pull requests, and ADRs: mainly English.
- Product and domain language: Spanish when useful.
- User-facing content: Spanish.
- Colombian domain context: Spanish.

### Rationale

This approach supports professional technical communication while preserving
the clarity and cultural relevance of the product domain.

### Consequences

- Some artifacts may contain both languages.
- Terminology must remain consistent across documents.
- Domain terms may require explicit definitions in the glossary.
- Translations must preserve meaning rather than only literal wording.

### Related Artifacts

- `README.md`
- `docs/03-supplementary-specification.md`
- `docs/04-glossary.md`

### Related ADR

Not required.

### Review Trigger

Review this decision if the project targets a different primary audience,
becomes internationally distributed, or requires full localization.

---

## DJ-003 — Follow a Product-Oriented and Iterative Engineering Approach

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Product

### Context

KUNNA is both a product concept and a software engineering portfolio project.

There is a risk of producing technical artifacts that demonstrate tools or
methods but do not contribute to user value or the product vision.

### Decision

The project will use a product-oriented and iterative engineering approach.

Engineering work should remain connected to:

- The product vision.
- User goals.
- Use cases.
- Risks.
- Prioritized backlog items.
- Testable outcomes.

The backlog will be treated as a living artifact rather than a fixed
long-term plan.

### Rationale

This approach keeps the project focused on solving meaningful user problems
while allowing product and technical understanding to evolve.

### Consequences

- Requirements and plans may be refined over time.
- Not all originally imagined features will necessarily be implemented.
- Work should be prioritized according to value, risk, and learning.
- Traceability must be maintained when decisions change.

### Related Artifacts

- `docs/00-vision.md`
- `docs/01-user-goals.md`
- `docs/05-risk-list.md`
- `docs/06-development-plan.md`
- `docs/07-development-framework.md`
- `backlog/product-backlog.md`

### Related ADR

Not required.

### Review Trigger

Review this decision if project work becomes disconnected from user value,
or if the backlog stops reflecting current product and engineering knowledge.

---

## DJ-004 — Use UML Selectively

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Modeling

### Context

UML can improve analysis, communication, and object-oriented design.

However, producing every possible UML diagram would create unnecessary
documentation and increase maintenance cost.

### Decision

KUNNA will use UML selectively when a diagram helps:

- Reduce ambiguity.
- Understand system behavior.
- Clarify domain concepts.
- Assign object responsibilities.
- Explain interactions.
- Support architecture reasoning.
- Communicate a design decision.

UML will not be treated as an end in itself.

### Rationale

The value of UML comes from supporting reasoning and communication, not from
maximizing the number of diagrams.

### Consequences

- Only useful diagrams will be created.
- Diagrams must remain consistent with the current project model.
- Some design reasoning may remain textual when a diagram adds little value.
- Outdated diagrams must be updated or removed.

### Related Artifacts

- `docs/02-use-case-model.md`
- `docs/07-development-framework.md`
- Future domain model.
- Future system sequence diagrams.
- Future interaction diagrams.

### Related ADR

Not required.

### Review Trigger

Review this decision when the project reaches domain modeling, architecture,
or object-oriented design activities.

---

## DJ-005 — Use Java First and Introduce Spring Boot Later

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Implementation

### Context

The project is intended to demonstrate Java and object-oriented software
engineering.

Starting immediately with a web framework could hide important domain,
object-oriented, and application design decisions behind framework
configuration.

### Decision

Java will be the primary implementation language.

The project should first establish:

- Domain concepts.
- Object responsibilities.
- Application boundaries.
- Core behavior.
- Tests.

Spring Boot may be introduced later when the project requires an API,
dependency injection, persistence integration, or web infrastructure.

### Rationale

This sequence supports deeper understanding of Java, object-oriented design,
and domain behavior before introducing framework complexity.

### Consequences

- The first implementation may be a framework-independent Java module.
- API development will occur after sufficient domain understanding exists.
- Future architectural decisions may require a dedicated ADR.
- Framework adoption should respond to product needs rather than portfolio
  fashion.

### Related Artifacts

- `docs/06-development-plan.md`
- `docs/07-development-framework.md`
- `backlog/product-backlog.md`

### Related ADR

A future ADR may be created when the architecture and Spring Boot adoption
decision become concrete.

### Review Trigger

Review this decision when an executable architecture is defined or when the
first API increment is planned.

---

## DJ-006 — Use a Professional GitHub Workflow

**Date:** 2026-08-01
**Status:** Accepted
**Category:** Process

### Context

KUNNA is intended to demonstrate not only final code but also a disciplined
and traceable engineering process.

Directly modifying `main` would reduce reviewability and make project history
less explicit.

### Decision

Each meaningful work item should follow this workflow:

1. Select or create a GitHub Issue.
2. Move the issue to `In Progress`.
3. Synchronize the local `main` branch.
4. Create a dedicated branch.
5. Modify the relevant artifact or code.
6. Validate the changes locally.
7. Create a focused commit.
8. Push the branch.
9. Open a pull request.
10. Connect the pull request to the issue.
11. Review the acceptance criteria.
12. Merge the pull request.
13. Synchronize local `main`.
14. Delete completed local and remote branches.
15. Confirm that the working tree is clean.

### Rationale

This workflow creates traceability between work items, branches, commits,
pull requests, and completed project outcomes.

### Consequences

- Small changes require additional workflow steps.
- Repository history becomes clearer and easier to review.
- Completed work is connected to explicit acceptance criteria.
- Branch hygiene must be maintained.

### Related Artifacts

- `.github/ISSUE_TEMPLATE/`
- `.github/pull_request_template.md`
- GitHub Issues.
- GitHub Projects.
- GitHub Pull Requests.

### Related ADR

Not required.

### Review Trigger

Review this decision if the project gains additional contributors or adopts
automated continuous integration and deployment workflows.

---

## DJ-007 — Use AI as a Support Tool with Human Responsibility

**Date:** 2026-08-01
**Status:** Accepted
**Category:** AI Governance

### Context

AI-assisted tools can accelerate research, drafting, analysis, modeling,
coding, testing, and documentation.

They can also produce incorrect, unverifiable, insecure, inappropriate, or
overengineered outputs.

### Decision

AI-assisted tools may support the KUNNA project, but they will not replace
human understanding, judgment, authorship, verification, or responsibility.

The project owner remains responsible for:

- Understanding every accepted artifact.
- Reviewing generated content.
- Validating technical decisions.
- Testing implementation results.
- Protecting sensitive information.
- Explaining project decisions.
- Approving final changes.

### Rationale

This approach uses AI productively while preserving professional integrity,
technical accountability, and authentic learning.

### Consequences

- AI-generated suggestions must be reviewed before acceptance.
- Outputs may be modified, rejected, or rewritten.
- Sensitive or private information must not be exposed unnecessarily.
- Portfolio evidence must not misrepresent authorship or understanding.
- Important AI-supported decisions should remain traceable.

### Related Artifacts

- `docs/08-ai-collaboration-policy.md`
- `docs/07-development-framework.md`
- `docs/05-risk-list.md`

### Related ADR

Not required.

### Review Trigger

Review this decision when new AI tools, autonomous agents, external data
sources, or automated repository actions are introduced.

## Journal Maintenance Rules

The journal should remain useful and concise.

When a new decision is added:

1. Assign the next sequential identifier.
2. Record the actual decision date.
3. Select an appropriate category.
4. Define the current status.
5. Explain the context and rationale.
6. Record consequences and trade-offs.
7. Link related artifacts.
8. Create an ADR only when justified.
9. Define a review trigger.
10. Update older entries when they are superseded.

Existing entries should not be silently rewritten when the decision changes.

Instead:

- Update the original entry status to `Superseded`.
- Add a new decision entry.
- Link the new entry to the previous decision.
- Explain why the decision changed.

## Traceability Rule

Every significant decision should be traceable to at least one of the
following:

- Product vision.
- User goal.
- Use case.
- Supplementary requirement.
- Risk.
- Backlog item.
- Issue.
- Pull request.
- ADR.
- Test or validation result.

This traceability helps demonstrate that KUNNA evolves through explicit
reasoning rather than disconnected implementation choices.

## Next Step

After completing this decision journal, the project should create:

- `decisions/ADR-0001-start-with-inception.md`

ADR-0001 will document in greater detail why KUNNA began with an Inception
Package before production implementation.
