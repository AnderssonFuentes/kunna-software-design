# 07 — Development Framework

## Document Purpose

This document defines the initial development framework for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to establish the engineering principles, process structure, modeling practices, quality controls, and collaboration rules that will guide the project from product understanding to implementation.

This framework complements the development plan by explaining not only what stages the project will follow, but also how engineering work will be performed within those stages.

## Framework Scope

This framework applies to:

- Product discovery and product definition.
- Requirements analysis.
- Use case modeling.
- Supplementary requirements.
- Risk management.
- Domain modeling.
- Object-oriented analysis and design.
- UML modeling.
- Architecture decisions.
- Java implementation.
- Future API development with Spring Boot.
- Testing.
- Technical documentation.
- Git and GitHub collaboration.
- AI-assisted work.

The framework is intentionally lightweight.

It provides enough structure to make the project traceable, explainable, and professionally credible without introducing unnecessary bureaucracy.

## Framework Overview

KUNNA follows a lightweight, iterative, risk-aware, use-case-driven, and object-oriented software engineering framework.

The framework is inspired by:

- Iterative and incremental development.
- The Unified Process.
- Craig Larman's object-oriented analysis and design approach.
- Use-case-driven development.
- UML modeling.
- Product-first thinking.
- Risk-driven planning.
- Architecture-aware development.
- Professional GitHub workflows.
- Continuous documentation.
- Selective use of design patterns and GRASP principles.

KUNNA does not attempt to reproduce the complete Unified Process.

Instead, it adapts useful practices to the scale, learning goals, portfolio purpose, and technical reality of the project.

## Core Engineering Principles

### 1. Product First

Engineering work must begin with the product problem, target users, expected outcomes, and product boundaries.

Technology is treated as a means to support the product rather than as the starting point of the project.

Before implementing a feature, the project should be able to explain:

- What problem is being addressed?
- Who is affected?
- What outcome is expected?
- Why is the feature valuable?
- How does it support KUNNA's product vision?

### 2. Documentation Before Irreversible Decisions

Important assumptions, requirements, risks, and decisions should be documented before they become difficult or expensive to change.

This does not mean documenting everything in advance.

Documentation should be created when it helps:

- Reduce ambiguity.
- Prevent rework.
- Explain decisions.
- Support traceability.
- Prepare implementation.
- Demonstrate engineering reasoning.

### 3. Iterative and Incremental Development

KUNNA will evolve through small, reviewable increments.

Each iteration should produce one or more verifiable outcomes, such as:

- A refined product artifact.
- A validated use case.
- A domain model improvement.
- A design decision.
- A Java implementation increment.
- A testable capability.
- A documented learning result.

The project should avoid large, unreviewed changes that combine unrelated concerns.

### 4. Risk-Driven Work

Work should be prioritized partly according to risk.

Higher-risk assumptions, architectural concerns, unclear requirements, and difficult technical decisions should be investigated before low-risk implementation details.

Risk management includes:

- Identifying risks.
- Estimating impact and probability.
- Defining mitigation actions.
- Monitoring status.
- Revising priorities when necessary.

### 5. Use-Case-Driven Analysis

User goals and use cases provide the main behavioral structure for the project.

Use cases help connect:

```text
User goals
    ↓
System behavior
    ↓
System operations
    ↓
Domain concepts
    ↓
Object responsibilities
    ↓
Software design
    ↓
Implementation
```

Not every requirement must be expressed as a use case.

Cross-cutting quality attributes and general constraints belong in the supplementary specification.

### 6. Selective Modeling

Models should be created when they improve understanding or reduce implementation risk.

The project may use:

- Use case models.
- Domain models.
- System sequence diagrams.
- Operation contracts.
- Interaction diagrams.
- Design class diagrams.
- Package diagrams.
- Architecture diagrams.
- State models when behavior requires them.

Not every feature requires every model.

The amount of modeling should be proportional to:

- Complexity.
- Risk.
- Learning value.
- Portfolio value.
- Need for communication.
- Need for traceability.

### 7. Object-Oriented Responsibility Assignment

Object-oriented design should focus on responsibilities rather than only on classes and syntax.

The project should ask:

- Which object should know this information?
- Which object should perform this behavior?
- Which object should create another object?
- How can coupling be reduced?
- How can cohesion be improved?
- Where should coordination occur?

GRASP principles may be used to support these decisions, including:

- Information Expert.
- Creator.
- Controller.
- Low Coupling.
- High Cohesion.
- Polymorphism.
- Pure Fabrication.
- Indirection.
- Protected Variations.

Patterns should be applied only when they solve a real design problem.

### 8. Traceability

Important project elements should be traceable from product intent to implementation.

A typical traceability path is:

```
Product vision
↓
User goals
↓
Use cases
↓
Supplementary requirements
↓
Domain concepts
↓
System operations
↓
Design decisions
↓
Code
↓
Tests
```

Traceability should be supported through:

- Consistent artifact names.
- Issue references.
- Pull request references.
- Closing keywords.
- Commit history.
- ADR references.
- Links between documentation files.

### 9. Evidence-Producing Work

Because KUNNA is also a professional portfolio project, the process should produce evidence of engineering ability.

Useful evidence includes:

- Clear requirements.
- Explicit decisions.
- UML models.
- Risk analysis.
- Iterative Git history.
- Pull requests.
- Conventional commits.
- Java implementation.
- Automated tests.
- Architecture explanations.
- Retrospectives.
- Trade-off analysis.

Portfolio value must not override product value.

Artifacts should exist because they support understanding, decisions, implementation, or learning.

## Process Structure

KUNNA uses four lightweight lifecycle phases inspired by the Unified Process.

These phases are not rigid sequential stages.

The project may revisit earlier artifacts when new information appears.

## Phase 1 — Inception

### Objective

Establish the initial direction, scope, vocabulary, risks, and working method of the project.

Main Questions

- What is KUNNA?
- Which problem does it address?
- Who are the primary users?
- What outcomes are expected?
- What is inside and outside the initial scope?
- What are the main risks?
- How will the project be organized?
- Why should implementation not begin immediately?

### Main Artifacts

- Initial README.
- Project vision.
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

### Exit Criteria

The Inception phase may be considered complete when:

- The product purpose is understandable.
- Target users are identified.
- Initial scope boundaries exist.
- Candidate use cases are documented.
- Important quality requirements are identified.
- Major risks are visible.
- The next iteration can be planned.
- The project has an explicit engineering workflow.

## Phase 2 — Elaboration

### Objective

Reduce the most important product, requirements, domain, and architecture risks.

- Expected Activities
- Refine priority use cases.
- Write detailed use case scenarios selectively.
- Identify system events.
- Create system sequence diagrams where useful.
- Define operation contracts for complex operations.
- Develop the domain model.
- Identify important business rules.
- Validate the conceptual architecture.
- Explore technical feasibility.
- Create architectural decision records.
- Build small technical or product prototypes when necessary.

### Expected Outputs

- Refined use cases.
- Initial domain model.
- System sequence diagrams.
- Selective operation contracts.
- Architecture baseline.
- Updated supplementary requirements.
- Updated risk list.
- Prioritized construction backlog.

### Exit Criteria

Elaboration may be considered complete when:

- The highest-risk product flows are understood.
- Core domain concepts are identified.
- Important system operations are known.
- Major architecture risks have been reduced.
- Construction work can begin without relying on major unresolved assumptions.

## Phase 3 — Construction

### Objective

Implement the software incrementally while preserving traceability, design quality, and testability.

### Expected Activities

- Implement domain behavior in Java.
- Apply object-oriented responsibility assignment.
- Create application services where coordination is required.
- Add automated tests.
- Refactor when design evidence justifies it.
- Record important architectural decisions.
- Maintain documentation and diagrams.
- Integrate persistence and external services incrementally.
- Introduce Spring Boot when the domain and application boundaries are sufficiently clear.

### Expected Outputs

- Working Java increments.
- Unit tests.
- Integration tests.
- Updated design models.
- Updated architecture documentation.
- Demonstrable use case slices.
- Stable pull requests and releases.

### Exit Criteria

Construction increments are complete when:

- The selected behavior works.
- Acceptance criteria are satisfied.
- Tests provide appropriate evidence.
- Important decisions are documented.
- Code and documentation remain synchronized.
- The increment can be explained by the project owner.

## Phase 4 — Transition

### Objective

Prepare the product increment for realistic use, demonstration, publication, or portfolio presentation.

### Expected Activities

- Stabilize the application.
- Correct defects.
- Improve usability and accessibility.
- Validate deployment.
- Review documentation.
- Prepare demonstrations.
- Improve onboarding instructions.
- Collect feedback.
- Identify the next iteration.

### Expected Outputs

- Deployable software.
- Updated README.
- Demonstration material.
- Known limitations.
- Release notes.
- Portfolio explanation.
- Next-step backlog.

## Requirements Framework

KUNNA separates different kinds of requirements.

### Product Requirements

Describe the problem, users, goals, expected outcomes, and scope.

Primary artifacts:

- Project vision.
- User goals.
- Product backlog.

### Behavioral Requirements

Describe interactions between actors and the system.

Primary artifacts:

- Use cases.
- System sequence diagrams.
- Operation contracts when necessary.

### Supplementary Requirements

Describe qualities, constraints, policies, and cross-cutting concerns.

Examples:

- Accessibility.
- Security.
- Performance.
- Reliability.
- Content quality.
- Privacy.
- Colombian domain considerations.
- Technology constraints.

### Primary artifact:

- Supplementary specification.

### Design Requirements

Describe decisions about responsibilities, collaboration, interfaces, architecture, and implementation boundaries.

Primary artifacts:

- Interaction diagrams.
- Design class diagrams.
- ADRs.
- Architecture documentation.

## Use Case Detail Strategy

Use cases should be refined selectively.

A use case may remain brief when:

- The flow is simple.
- The behavior is low risk.
- The intent is already clear.
- Additional detail would not improve implementation.

A use case should receive more detail when:

- It represents a core product flow.
- It contains alternatives or exceptions.
- It introduces important business rules.
- It affects sensitive information.
- It creates architectural risk.
- It is difficult to explain or test.

## Operation Contract Strategy

Operation contracts may be created for system operations that require greater analytical precision.

A contract may include:

- Operation name.
- Parameters.
- Related use case.
- Preconditions.
- Postconditions.

Postconditions should describe changes in domain state, such as:

- Creation or deletion of instances.
- Modification of attributes.
- Formation or removal of associations.

Contracts describe what becomes true after an operation.

They should not describe implementation steps.

Contracts will be used selectively in KUNNA rather than for every system operation.

## Architecture Strategy

Architecture should emerge through deliberate decisions rather than premature framework configuration.

The initial architecture should prioritize:

- Clear domain concepts.
- Separation of responsibilities.
- Testability.
- Low coupling.
- High cohesion.
- Replaceable technical details.
- Incremental evolution.
- Explainable boundaries.

Likely architectural concerns include:

- Domain logic.
- Application coordination.
- User interface.
- Persistence.
- External services.
- Security.
- Content delivery.
- Future API boundaries.

Spring Boot should be introduced when it supports a defined application need, not merely because it is part of the intended technology stack.

## Implementation Strategy

Implementation should begin with the smallest useful vertical or behavioral slice.

A typical implementation path may be:

```
Use case
↓
System operation
↓
Domain behavior
↓
Application coordination
↓
Infrastructure integration
↓
Automated verification
```

Java implementation should prioritize:

- Clear names.
- Explicit responsibilities.
- Small cohesive units.
- Appropriate encapsulation.
- Tests around important behavior.
- Refactoring based on evidence.
- Avoidance of unnecessary abstractions.

## Testing Framework

Testing should be proportional to risk and behavior.

Unit Testing

Used for:

- Domain rules.
- Calculations.
- Validation.
- Object behavior.
- Small isolated components.

### Integration Testing

Used for:

- Persistence.
- External services.
- Framework integration.
- API behavior.
- Component collaboration.

### Acceptance-Oriented Testing

Used to verify:

- Use case outcomes.
- Acceptance criteria.
- Important user flows.
- Product rules.

### Documentation Review

Documentation should also be reviewed for:

- Internal consistency.
- Traceability.
- Ambiguity.
- Outdated assumptions.
- Alignment with the product vision.

### Git and GitHub Workflow

KUNNA uses the following standard workflow:

```
Issue
↓
Project board status
↓
Feature or documentation branch
↓
Focused commits
↓
Push
↓
Pull request
↓
Review
↓
Merge into main
↓
Issue closure
↓
Branch deletion
```

### Branch Naming

Examples:

```
docs/initial-project-vision
docs/initial-use-case-model
docs/initial-development-framework
feature/save-bookmark
test/bookmark-service
refactor/content-domain
```

### Commit Style

KUNNA uses Conventional Commit-style messages.

Examples:

```
docs: create initial development framework
feat: add bookmark creation behavior
test: cover bookmark validation
refactor: simplify content selection
fix: prevent duplicate bookmarks
```

### Pull Request Rules

A pull request should:

- Have a clear title.
- Summarize the change.
- Reference the related issue.
- Identify the change type.
- Confirm acceptance criteria.
- Avoid unrelated modifications.
- Be reviewed before merging.
- Delete the branch after merge when appropriate.

### Work Item Types

**Product Issue**

Used for:

- Product definition.
- Requirements.
- User goals.
- Use cases.
- Scope decisions.
- Documentation tied to product understanding.

### Technical Task

Used for:

- Repository configuration.
- Tooling.
- Implementation.
- Refactoring.
- Tests.
- Build configuration.
- Infrastructure.

### Decision Task

Used when an important decision requires explicit analysis.

A decision task may result in:

- An ADR.
- A decision journal entry.
- A documented trade-off.
- A rejected alternative.

### Decision Management

Important decisions should be documented when they:

- Affect architecture.
- Introduce a long-term constraint.
- Change project scope.
- Select a significant technology.
- Reject a plausible alternative.
- Influence several future work items.
  Are difficult to reverse.

ADRs should describe:

- Context.
- Decision.
- Alternatives.
- Consequences.
- Status.

Smaller decisions may be recorded in the decision journal.

### AI-Assisted Work

AI tools may support:

- Drafting.
- Reviewing.
- Comparing alternatives.
- Explaining concepts.
- Identifying omissions.
- Generating test ideas.
- Refactoring suggestions.
- Documentation improvement.

AI-generated output must not be accepted automatically.

The project owner must:

- Understand the result.
- Verify technical claims.
- Check consistency with previous artifacts.
- Remove unsupported assumptions.
- Preserve authorship and accountability.
- Be able to explain the final decision.

Detailed rules will be defined in the AI collaboration policy.

### Quality Gates

**Artifact Quality Gate**

A documentation artifact is ready when:

- Its purpose is clear.
- It supports the current phase.
- It is internally consistent.
- It references relevant previous artifacts.
- It avoids unsupported assumptions.
- It identifies unresolved questions where necessary.
- It prepares the next relevant activity.

### Implementation Quality Gate

A software increment is ready when:

- The intended behavior works.
- Acceptance criteria are satisfied.
- Important tests pass.
- Code is understandable.
- Responsibilities are reasonably assigned.
- No unrelated changes are included.
- Documentation is updated when necessary.
- The project owner can explain the implementation.

### Pull Request Quality Gate

A pull request is ready to merge when:

- The change is focused.
- The diff has been reviewed.
- No unresolved conflicts exist.
- Acceptance criteria are met.
- The related issue is referenced.
- Important trade-offs are documented.
- The branch is synchronized sufficiently with main.

### Definition of Done

A KUNNA work item is considered done when:

- The expected outcome exists.
- Acceptance criteria are satisfied.
- Relevant documentation or code is committed.
- The pull request has been merged.
- The related issue is closed.
- The project board reflects the final status.
- Local main is updated.
- The working tree is clean.
- Temporary branches are removed when appropriate.
- The project owner understands and can explain the result.

### Practices to Avoid

KUNNA should avoid:

- Coding before understanding the product problem.
- Creating every possible UML diagram.
- Applying patterns without a real design problem.
- Adding frameworks before they are needed.
- Treating documentation as a one-time activity.
- Producing artifacts only for appearance.
- Combining many unrelated changes in one pull request.
- Allowing AI output to replace engineering judgment.
- Building the complete product in one large iteration.
- Designing for hypothetical future scale without evidence.
- Confusing UI screens with domain concepts.
- Confusing database tables with the domain model.
- Confusing use cases with interface navigation.

### Framework Evolution

This framework is expected to evolve.

Changes may be introduced when:

- The product vision changes.
- New risks appear.
- The architecture becomes clearer.
- Implementation evidence reveals a better practice.
- The current process creates unnecessary overhead.
- New team members or contributors require clearer rules.

Significant changes to the framework should be documented through an issue, pull request, or ADR.

### Portfolio Value

This framework helps KUNNA demonstrate:

- Product-oriented engineering.
- Requirements discipline.
- Iterative development.
- Risk management.
- Object-oriented analysis and design.
- Selective UML usage.
- Architecture reasoning.
- Professional GitHub practices.
- Testing awareness.
- Traceability.
- Responsible AI collaboration.
- Ability to explain technical decisions.

### Next Step

After completing this development framework, the project should continue with the initial product backlog.

The backlog will translate the product vision, user goals, use cases, risks, and engineering plan into prioritized and actionable work items.
