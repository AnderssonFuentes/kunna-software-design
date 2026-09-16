# 00 — Project Vision

## Product Name

KUNNA

## Document Purpose

This document defines the product vision baseline for KUNNA.

The vision was initially established during the **I1 — Inception Package** and is maintained as the project evolves through **I2 — Elaboration** and subsequent work.

Its purpose is to clarify:

- What KUNNA is intended to become.
- Who the product is intended to support.
- Which problem and user needs are currently being explored.
- Which product capabilities originated in the original UX/UI prototype.
- Which assumptions remain hypotheses rather than validated requirements.
- How product reasoning should guide engineering decisions.

This document connects the original UX/UI prototype with the current software engineering process.

It is not intended to define every requirement, architecture decision, or implementation detail in advance.

## Product Idea

KUNNA is a digital product concept intended primarily to support mothers, fathers, and caregivers with accessible information related to children's rights, positive parenting, and daily caregiving practices.

The core product domain currently includes:

- Derechos de niñas y niños.
- Crianza positiva.
- Daily caregiving practices.
- Practical caregiver-oriented information.

The original UX/UI prototype also explored capabilities such as:

- Daily tips.
- Audio content.
- Bookmarks.
- Downloads.
- Search.
- User profiles.
- Content sharing.

These capabilities are treated as **candidate product scope and product hypotheses**.

Their presence in the original prototype does not mean that they are validated requirements or guaranteed implementation commitments.

## Vision Statement

KUNNA aims to provide caregivers with practical, accessible, understandable, and responsibly handled information related to children's rights, positive parenting, and caregiving.

From a software engineering perspective, KUNNA is being evolved from an original UX/UI prototype into an iterative, risk-aware, use-case-driven, and object-oriented software engineering project.

The objective is not merely to reproduce the original interface or accumulate project artifacts.

The objective is to create credible and traceable engineering evidence through product reasoning, requirements analysis, selective modeling, architecture decisions, implementation, automated testing, and iterative validation.

## Background

KUNNA started as a UX/UI prototype created several years ago during a design and user experience learning process.

The original prototype won first place in a course and included a visual flow focused on caregivers and child-related content.

This repository does not treat KUNNA as an old application that must simply be recreated.

Instead, the original prototype provides historical product context that can be reviewed, challenged, refined, or discarded as the software engineering work produces better evidence.

The project also serves as professional software engineering evidence for learning and employability.

Portfolio value should result from the engineering work that actually occurs rather than determine product requirements, architecture, technologies, or implementation scope.

## Problem Hypothesis

The initial product hypothesis is that caregivers may need clear, practical, and trustworthy information about children's rights, positive parenting, and daily care practices.

Potential difficulties identified during I1 include information that may be:

- Fragmented across different sources.
- Difficult to understand.
- Too general or disconnected from daily caregiving situations.
- Hard to revisit when needed.
- Not presented in a format suitable for quick consultation.

These statements represent the current product baseline.

They should not be interpreted as completed user research or validated market evidence.

Future research or product evidence may confirm, refine, narrow, or challenge them.

## Target Users

The candidate primary users identified during I1 are:

- Mothers.
- Fathers.
- Caregivers.
- People responsible for the daily care and protection of children.

In Spanish product and domain language, these users may be described as:

- Madres.
- Padres.
- Cuidadores.
- Personas responsables del cuidado diario de niñas y niños.

The exact boundaries of the target audience may be refined when stronger product evidence becomes available.

## Candidate User Needs

Initial candidate user needs derived from the product concept and original prototype include:

- Accessing understandable content about children's rights.
- Consulting practical parenting information.
- Finding relevant information efficiently.
- Returning to useful content later.
- Accessing information through alternative formats when appropriate.
- Sharing useful information when that capability is justified.

More specific capabilities such as bookmarking, audio playback, downloads, profiles, or sharing remain hypotheses until they are justified by the selected product behavior and available evidence.

## Expected Product Outcome

The long-term product direction is to make relevant caregiving information easier to understand, consult, and use responsibly.

The product outcome is not assumed to be a specific interface, platform, backend, or technical architecture.

Capabilities from the original prototype should be preserved only when current product reasoning and evidence justify them.

Content credibility is particularly important because the product domain involves children, caregiving, and rights.

When authoritative or user-facing claims are introduced, appropriate source provenance and domain validation should remain traceable.

## Expected Engineering Outcome

The engineering objective is to demonstrate the ability to evolve an initial product concept through disciplined software engineering.

Relevant evidence may include:

- Product reasoning.
- User goal analysis.
- Use-case-driven development.
- Supplementary requirements.
- Risk identification and reassessment.
- Domain modeling.
- Selective UML.
- Object-oriented analysis and design.
- Architecture hypotheses and decisions.
- Progressive Java implementation.
- Automated testing.
- Traceability between requirements, decisions, code, tests, and evidence.
- Iterative review and refinement.

Engineering artifacts should be created when they support an actual product, analysis, design, validation, or communication need.

Completeness of documentation is not an objective by itself.

## I1 — Inception Baseline

The **I1 — Inception Package** established the initial product and engineering foundation for KUNNA.

It included:

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

I1 was completed and closed on **2026-08-02**.

Its purpose was to establish enough shared understanding to continue iteratively rather than to define the complete product or architecture upfront.

## Current Phase

The project is currently in:

**I2 — Elaboration**

I2 focuses on reducing significant product, requirements, domain, and architecture risks through focused analysis and executable evidence.

The current direction is to:

- Review and refine the I1 baseline where necessary.
- Select one architecturally significant use case.
- Refine only the behavior and supplementary requirements relevant to that slice.
- Create focused domain and system-operation analysis.
- Formulate an architecture hypothesis.
- Implement a small executable Java vertical slice.
- Add meaningful automated tests.
- Evaluate the resulting evidence.
- Reassess risks, assumptions, architecture decisions, and backlog priorities.

Elaboration is therefore **not analysis-only**.

Executable evidence may be produced before broader Construction work begins.

## Current Product Scope Position

The current product scope remains intentionally provisional.

The project should not assume that every capability from the original prototype belongs in the final product.

Candidate capabilities include:

- Viewing relevant content.
- Viewing daily tips.
- Browsing categories.
- Searching content.
- Saving content.
- Playing audio content.
- Downloading resources.
- Sharing content.
- Managing a profile.

The selected I2 use case will determine which subset requires deeper analysis.

Scope should be refined through evidence rather than by attempting to implement every historical prototype capability.

## Not Currently Assumed for I2

The following capabilities or technical mechanisms are not automatically required during I2:

- Production-ready backend.
- Mandatory Spring Boot API.
- Production database.
- Authentication.
- Password recovery.
- User registration.
- Full content management system.
- Mobile application.
- Production deployment.
- Final UI redesign.
- Production-scale infrastructure.

Any of these may be introduced later if a demonstrated product, delivery, integration, security, or architecture need justifies them.

## Strategic Direction

KUNNA follows an iterative, product-oriented, risk-aware, use-case-driven, and evidence-driven engineering approach.

This means:

- The problem should be understood before committing to a solution.
- User outcomes should guide implementation decisions.
- Product assumptions should remain distinguishable from validated requirements.
- The original prototype should provide context rather than dictate implementation.
- Documentation and implementation should complement each other.
- Modeling should be selective and purpose-driven.
- Architecture should evolve progressively.
- Technologies should be introduced only when justified.
- Executable feedback should be used to challenge assumptions.
- Important decisions should remain traceable.
- AI may support analysis, drafting, review, and implementation, but final responsibility remains human.
- Code should not be accepted if the project owner cannot explain its purpose and behavior.

The project does not require every possible document, UML model, or design artifact before implementation can begin.

## Relationship with the Project Lifecycle

This vision originated during Inception but remains a living product baseline.

The transition from I1 to I2 does not invalidate the original vision.

Instead, Elaboration provides an opportunity to test and refine assumptions established during Inception.

Requirements, use cases, domain concepts, architecture assumptions, and even parts of the product vision may evolve when stronger evidence becomes available.

Normal refinement during I2 does not require reopening the completed I1 milestone.

## Success Criteria for This Vision

This vision remains useful if it helps answer:

- What is KUNNA?
- Why does KUNNA exist?
- Who is KUNNA intended to support?
- What problem hypothesis is currently being explored?
- Which ideas come from the original prototype?
- Which capabilities remain hypotheses?
- What is the current product and engineering direction?
- Which decisions are intentionally deferred?
- How should implementation decisions remain connected to product reasoning and evidence?

## Open Questions

The following questions remain relevant during Elaboration:

- Which architecturally significant use case should drive the current I2 slice?
- Which user need does that use case primarily address?
- Which supplementary requirements materially affect that behavior?
- Which domain concepts and system operations are necessary for the selected slice?
- Which parts of the original UX/UI prototype remain useful product hypotheses?
- Which prototype assumptions should be discarded or deferred?
- What content evidence or provenance is required for the selected behavior?
- What is the smallest executable Java vertical slice that can provide meaningful engineering evidence?
- Can the selected behavior be validated without persistence?
- Does the selected behavior require authentication?
- Which architecture assumptions should be tested through executable evidence?
- Which technologies, if any, are actually required to validate the selected behavior?

These questions should be narrowed progressively rather than answered globally in advance.

## Language Note

Technical documentation, repository structure, code, commits, branches, issues, pull requests, and ADRs are mainly written in English.

Product and domain concepts related to Colombian caregivers, children's rights, and user-facing content may be expressed in Spanish when this improves clarity.

This hybrid language approach should preserve technical consistency while respecting the product's domain context.

## Current Vision Position

The original KUNNA concept remains the product starting point, not a fixed implementation specification.

I1 established the initial vision and engineering foundation.

I2 now uses that baseline to determine which product behavior deserves deeper analysis and executable validation.

The project should continue evolving through evidence, focused risk reduction, and traceable engineering decisions rather than through exhaustive documentation or predetermined technology choices.
