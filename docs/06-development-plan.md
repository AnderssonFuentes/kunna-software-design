# 06 — Development Plan

## Document Purpose

This document defines the initial development plan for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to describe how the project will move from product understanding to software engineering artifacts, design decisions, UML modeling, Java implementation, and future API development.

This plan keeps the project organized, realistic, and suitable as professional software engineering portfolio evidence.

## Project Context

KUNNA is a personal software engineering project based on an original UX/UI prototype.

The goal is not only to build an application, but to document a complete engineering process that demonstrates:

- Product thinking.
- Requirements analysis.
- Use case modeling.
- Supplementary requirements.
- Risk identification.
- UML and domain modeling.
- Object-oriented analysis and design.
- Design decisions.
- Java implementation.
- Future API development with Spring Boot.
- Professional GitHub workflow.

## Current Phase

The project is currently in:

**I1 — Inception Package**

This phase focuses on understanding the product, defining the initial scope, documenting the problem, identifying users, clarifying requirements, and preparing the repository before writing production code.

The main goal of the Inception Package is to answer:

- What is KUNNA?
- Who is it for?
- What problem does it address?
- What should the first version focus on?
- What risks should be controlled?
- What documentation is needed before implementation?
- What engineering evidence should the repository show?

## Development Strategy

KUNNA follows a documentation-first and product-first development strategy.

This means that the project does not start directly with code. Instead, it starts with a structured understanding of the product, the users, the requirements, and the engineering decisions needed to build it correctly.

The strategy is based on the following principles:

- Understand the product before implementing features.
- Define user goals before writing use cases.
- Define use cases before designing internal logic.
- Define constraints and quality attributes before implementation.
- Use UML selectively when it improves clarity.
- Use Java implementation only after the main analysis artifacts are clear.
- Keep every artifact connected to the product vision.
- Avoid overengineering and unnecessary documentation.

## Development Phases

The project will be developed through incremental phases.

| Phase | Name              | Main Purpose                        | Main Output                                                      |
| ----- | ----------------- | ----------------------------------- | ---------------------------------------------------------------- |
| I1    | Inception Package | Define the product foundation       | Vision, goals, use cases, risks, backlog, glossary, decisions    |
| E1    | Elaboration       | Analyze the domain and architecture | Domain model, system operations, contracts, design direction     |
| C1    | Construction      | Implement the first Java version    | Core Java classes, services, tests, documentation                |
| C2    | API Construction  | Expose functionality through an API | Spring Boot API, endpoints, validation, persistence              |
| T1    | Transition        | Prepare portfolio presentation      | README, screenshots, diagrams, deployment notes, lessons learned |

## Phase I1 — Inception Package

The Inception Package is the current focus.

Its purpose is to create the initial project foundation before moving into deeper analysis or implementation.

The expected artifacts are:

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

The phase is complete when these artifacts describe a clear, coherent, and realistic foundation for the project.

## Phase E1 — Elaboration

The Elaboration phase will start after the Inception Package is complete.

Its purpose is to transform the initial product understanding into more detailed software engineering artifacts.

This phase may include:

- Domain model.
- Conceptual classes.
- Associations.
- Attributes.
- System sequence diagrams.
- System operations.
- Operation contracts.
- Initial design model.
- Selected GRASP pattern analysis.
- Architecture decisions.

This phase will use Craig Larman's object-oriented analysis and design approach selectively.

The goal is not to reproduce the entire book process mechanically. The goal is to use the parts that help clarify the design of KUNNA.

## Phase C1 — Java Construction

The Java Construction phase will focus on implementing the first version of the domain logic.

This phase may include:

- Java domain classes.
- Services or use case handlers.
- Basic validation.
- Unit tests.
- Simple command-line or test-based interaction.
- Object-oriented design improvements.
- Documentation of implementation decisions.

The first Java version should prioritize clarity over complexity.

The goal is to show that the analysis artifacts can lead to understandable code.

## Phase C2 — API Construction

The API Construction phase will introduce Spring Boot after the core domain understanding is clear.

This phase may include:

- REST API structure.
- Controllers.
- Services.
- DTOs.
- Validation.
- Error handling.
- Persistence.
- API documentation.
- Integration with the domain model.

Spring Boot should not be introduced too early. It will be used when the project already has enough product and domain clarity.

## Phase T1 — Transition and Portfolio Preparation

The Transition phase will prepare the project as professional portfolio evidence.

This phase may include:

- Final README improvements.
- Architecture summary.
- Screenshots.
- Diagrams.
- Project walkthrough.
- Lessons learned.
- Technical decisions summary.
- Professional narrative for GitHub and LinkedIn.
- Explanation of the software engineering process.

The goal is to make the repository understandable for reviewers, recruiters, mentors, or technical interviewers.

## Development Workflow

The project uses a professional GitHub-based workflow.

Each relevant change should follow this process:

1. Select one issue from the GitHub Project board.
2. Move the issue to **In Progress**.
3. Create a dedicated branch from `main`.
4. Work on only one artifact or topic at a time.
5. Commit the change with a clear Conventional Commit message.
6. Push the branch to GitHub.
7. Create a pull request connected to the issue.
8. Review the changes.
9. Merge the pull request into `main`.
10. Pull the latest `main` branch locally.
11. Delete the completed local and remote branch.
12. Move the issue to **Done**.

## Branch Naming Rule

Branches should describe the type and purpose of the work.

Examples:

- `docs/initial-readme`
- `docs/initial-project-vision`
- `docs/initial-user-goals`
- `docs/initial-use-case-model`
- `docs/initial-supplementary-specification`
- `docs/initial-glossary`
- `docs/initial-risk-list`
- `docs/initial-development-plan`

For future implementation work, branch names may use prefixes such as:

- `feat/`
- `fix/`
- `test/`
- `refactor/`
- `docs/`

## Commit Rule

Commits should use clear Conventional Commit messages.

Examples:

- `docs: improve initial README`
- `docs: write initial project vision`
- `docs: define initial user goals`
- `docs: create initial use case model`
- `docs: write supplementary specification`
- `docs: create initial glossary`
- `docs: create initial risk list`
- `docs: create initial development plan`

The commit message should explain what changed, not the entire history of the task.

## Pull Request Rule

Each pull request should be connected to a GitHub issue.

The pull request description should include:

- Summary.
- Related issue.
- Type of change.
- Acceptance criteria.
- Notes.

The pull request should use closing keywords such as:

```text
Closes #issue-number
```

This allows GitHub to close the related issue automatically after the pull request is merged.

## Definition of Done

An artifact or task is considered done when:

- The document or change is completed.
- The content is connected to KUNNA's product vision.
- The result is clear enough to be understood later.
- The change is committed with a clear message.
- The branch is pushed to GitHub.
- A pull request is created.
- The pull request is merged into main.
- The related issue is closed.
- The project board is updated.
- The local repository is synchronized with GitHub.
- The temporary branch is deleted.

## Use of UML and Larman's Approach

KUNNA will use UML and Craig Larman's object-oriented analysis and design approach selectively.

The project may use concepts such as:

- Use cases.
- System operations.
- Operation contracts.
- Domain model.
- Conceptual classes.
- Associations.
- Attributes.
- Postconditions.
- Interaction diagrams.
- GRASP principles.
- Design patterns.

However, these tools will only be used when they help explain, analyze, or design the system.

The project will avoid creating UML diagrams or contracts only for formality.

## Scope Control

To keep the project realistic, the following limits apply:

- Do not start coding before the Inception Package is complete.
- Do not introduce Spring Boot before the core domain understanding is clear.
- Do not create diagrams that do not support analysis or design.
- Do not document features that are not connected to user goals.
- Do not expand the product scope without updating the backlog and risk list.
- Do not treat the original UX/UI prototype as final implementation scope.
- Do not prioritize visual polish before software engineering clarity.
- Initial Work Order

## The recommended work order is:

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

This order helps the project move from general understanding to more detailed engineering planning.

## Portfolio Value

This development plan supports the professional value of the repository.

It shows that KUNNA is not only a personal idea, but a structured software engineering project with:

- Clear planning.
- Traceable decisions.
- Incremental progress.
- Requirements discipline.
- Technical restraint.
- GitHub workflow practice.
- Connection between product thinking and implementation.

## Next Step

After this development plan, the project should continue with the development framework.

The development framework will explain the engineering approach, methods, concepts, and practices that guide the project in more detail.
