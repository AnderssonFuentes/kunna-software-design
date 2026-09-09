# 03 — Supplementary Specification

## Document Purpose

This document defines the supplementary specification baseline for KUNNA.

The specification was initially created during the **I1 — Inception Package** and is now reviewed as part of **I2 — Elaboration**.

The purpose of this artifact is to document requirements, constraints, quality attributes, and general rules that are not fully described by individual use cases.

This document complements:

- `README.md`
- `docs/00-vision.md`
- `docs/01-user-goals.md`
- `docs/02-use-case-model.md`

The requirements recorded here originated as an initial I1 baseline. They should not all be interpreted as validated, equally important, or automatically applicable to the current I2 slice.

Detailed refinement should remain focused on the architecturally significant use case selected for I2 and on the supplementary requirements that materially affect that slice.

## What Is a Supplementary Specification?

A supplementary specification captures requirements that apply across the system or affect the product as a whole.

Use cases describe user-system interactions.

The supplementary specification describes additional concerns such as:

- Usability.
- Accessibility.
- Reliability.
- Performance expectations.
- Security considerations.
- Content rules.
- Language rules.
- Technical constraints.
- Documentation rules.
- Implementation assumptions that require validation.

## System Under Design

The system under design is:

**KUNNA**

KUNNA is a digital product concept intended primarily to support mothers, fathers, and caregivers.

The original UX/UI prototype explored capabilities related to children's rights, positive parenting, daily tips, audio content, bookmarks, downloads, search, profiles, and content sharing.

These capabilities remain candidate product scope unless they are supported by current product reasoning and selected for further refinement or implementation.

## Current Phase

The project is currently in:

**I2 — Elaboration**

The previous milestone, **I1 — Inception Package**, was completed and closed.

I2 focuses on reducing significant product, requirements, domain, and architecture risks through focused analysis and executable evidence.

The current milestone is expected to:

- Review and refine the I1 baseline.
- Select one architecturally significant use case.
- Refine only the behavior and supplementary requirements relevant to that slice.
- Create focused domain and system-operation analysis.
- Formulate an architecture hypothesis.
- Implement a small executable Java vertical slice.
- Add meaningful automated tests.
- Evaluate the resulting evidence.
- Reassess risks and architecture assumptions before considering Construction.

Executable work during Elaboration is intended to validate engineering decisions. It does not imply that KUNNA is production-ready or that broad infrastructure is required.

## Scope of This Specification

This document contains the initial cross-cutting requirements and constraints established during I1, together with the minimum updates required to keep the baseline coherent during I2.

The requirements are not final.

Some remain hypotheses or preliminary quality expectations and may be refined, narrowed, deferred, or superseded when the selected I2 use case provides better evidence.

The I2 baseline review does not attempt to rewrite every supplementary requirement in advance.

## Functional Context

The current use case model identifies the following candidate use cases:

- UC-01 — View Content.
- UC-02 — View Daily Tip.
- UC-03 — Search Content.
- UC-04 — Bookmark Content.
- UC-05 — View Saved Content.
- UC-06 — Play Audio Content.
- UC-07 — Download Resource.
- UC-08 — Share Content.
- UC-09 — Manage Profile.
- UC-10 — Browse Content Categories.

This supplementary specification defines cross-cutting requirements that may affect several of these use cases.

The presence of a use case in this list does not mean that it has been selected for the current I2 vertical slice.

## Usability Requirements

### SUP-01 — Clear and Accessible Language

KUNNA should use clear, simple, and understandable language for caregivers.

Product and domain content should avoid unnecessary legal, technical, or academic complexity.

#### Rationale

The product is intended for mothers, fathers, and caregivers who may need practical guidance in daily situations.

---

### SUP-02 — Simple Navigation

KUNNA should provide simple navigation between content, categories, daily tips, saved content, audio, downloads, search, profile, and sharing options when those capabilities are part of the implemented product scope.

#### Rationale

Caregivers may need to find information quickly and without friction.

---

### SUP-03 — Quick Consultation

KUNNA should support short and practical interactions.

Users should be able to consult relevant content without completing long processes.

#### Rationale

Caregiving contexts may require fast access to information.

---

## Accessibility Requirements

### SUP-04 — Readable Content

Text content should be presented in a readable format with clear hierarchy, spacing, and structure.

#### Rationale

The product should support comfortable reading and understanding.

---

### SUP-05 — Audio as an Accessibility Support

Audio content may be used to provide an additional way to consume information.

#### Rationale

Some caregivers may prefer listening or may not be able to read at a specific moment.

---

### SUP-06 — Inclusive Interaction Design

Future UI implementation should consider inclusive interaction patterns such as visible actions, readable labels, and consistent navigation.

#### Rationale

The original UX/UI prototype should be reinterpreted with accessibility and usability in mind.

## Language Requirements

### SUP-07 — Technical Language Rule

Technical project language should be mainly English.

This applies to:

- Repository documentation.
- Commits.
- Branches.
- Issues.
- Pull requests.
- ADRs.
- Code.
- Technical notes.

---

### SUP-08 — Product and Domain Language Rule

Product and domain language should be mainly Spanish when it refers to user-facing content, Colombian caregiving context, or child-rights content.

This applies to:

- User-facing content.
- Product copy.
- Child rights concepts.
- Positive parenting content.
- Domain examples.
- Colombian context.

---

### SUP-09 — Hybrid Documentation Rule

Some documents may include both English and Spanish when useful.

Technical explanation should remain mainly English, while domain examples may remain in Spanish.

#### Rationale

KUNNA is both a software engineering portfolio project and a product idea connected to a Spanish-speaking domain context.

## Content Requirements

### SUP-10 — Content Should Be Practical

KUNNA content should be practical and connected to real caregiving situations.

#### Rationale

The value of the product depends on whether caregivers can apply or understand the information.

---

### SUP-11 — Content Should Be Trustworthy

KUNNA should treat child-rights and parenting content as sensitive and important.

Content sources should be reviewed carefully before authoritative or user-facing claims are accepted.

#### Rationale

The product domain involves children, care, and rights. Inaccurate content could be harmful.

---

### SUP-12 — Content Should Be Organized by Topics or Categories

Content should be organized in a way that supports browsing and searching when those capabilities are part of the selected product scope.

Possible initial categories may include:

- Derechos de niñas y niños.
- Crianza positiva.
- Cuidado diario.
- Tips diarios.
- Recursos.
- Audio content.

---

### SUP-13 — Content Should Support Reuse

Useful content should be easy to save, revisit, share, or download when those capabilities are appropriate and included in the implemented scope.

#### Rationale

Caregivers may need to return to important content later.

## Security and Privacy Requirements

### SUP-14 — No Real Sensitive Data in Current Engineering Work

Current analysis, experiments, tests, and executable validation should avoid real personal or sensitive data.

#### Rationale

I2 does not require production user data. Examples and tests can use fictitious, anonymized, or synthetic information while privacy needs remain under analysis.

---

### SUP-15 — Future Profile Data Must Be Treated Carefully

If user profiles are implemented in a future phase, profile data should be handled with privacy and security considerations.

#### Rationale

The product may eventually include saved content, preferences, or user information.

---

### SUP-16 — Authentication Is Not Currently Assumed

Authentication, password recovery, account management, and user registration are not automatically required for the current I2 slice.

If the selected use case or validation strategy demonstrates a need for authentication, that need should be analyzed explicitly before implementation.

#### Rationale

Authentication introduces security, privacy, persistence, and architecture consequences that should not be adopted without demonstrated need.

## Reliability Requirements

### SUP-17 — Content Access Should Be Predictable

When implemented, users should be able to access available content consistently.

#### Rationale

The product is intended to provide support and guidance. Broken content access would reduce trust.

---

### SUP-18 — Saved Content Should Be Stable

If bookmark functionality is implemented, saved content should remain available within the expected persistence model.

#### Rationale

Saved content only creates value if users can reliably return to it.

## Performance Requirements

### SUP-19 — Basic Content Interactions Should Be Fast

Implemented content interactions should prioritize responsive access when performance is relevant to the selected use case.

#### Rationale

Caregivers may need quick consultation.

---

### SUP-20 — Performance Requirements Are Preliminary

Exact performance targets are not yet defined.

#### Rationale

Meaningful targets should be derived from the selected behavior, architecture hypothesis, delivery context, and available evidence rather than invented in advance.

## Technical Constraints

### SUP-21 — Executable Validation Is Allowed During Elaboration

I2 may include a small executable Java vertical slice and meaningful automated tests.

This work is intended to validate analysis, design, architecture assumptions, and technical risks.

It does not require production-ready implementation.

#### Rationale

Executable evidence can expose incorrect assumptions earlier than analysis or documentation alone.

---

### SUP-22 — Implementation Should Be Progressive and Evidence-Driven

Java is the primary implementation language.

The first I2 executable slice should use the smallest technically sufficient solution that supports the selected use case and validation strategy.

Frameworks, APIs, persistence, authentication, databases, or other infrastructure should be introduced only when a demonstrated product, delivery, integration, or architecture need justifies them.

#### Rationale

The project should develop technical capability while avoiding premature complexity and predetermined architecture.

---

### SUP-23 — Code Must Be Explainable

No code should be accepted if the project owner cannot explain it.

#### Rationale

The project is intended to demonstrate real learning, not only generated output.

---

### SUP-24 — GitHub Is the Project Workspace

GitHub is the central workspace for:

- Repository files.
- Issues.
- Project board.
- Milestones.
- Pull requests.
- Labels.
- Decision records.
- Portfolio evidence.

## Documentation Requirements

### SUP-25 — Each Major Artifact Should Be Connected to an Issue

Every important document or change should be connected to a GitHub Issue.

#### Rationale

This creates traceability between work items and project artifacts.

---

### SUP-26 — Each Important Change Should Use a Branch

Changes should be made in a dedicated branch before being merged into `main`.

#### Rationale

This supports a professional development workflow.

---

### SUP-27 — Pull Requests Should Be Used for Integration

Changes should be integrated into `main` through Pull Requests.

#### Rationale

Pull Requests create review points and professional evidence.

---

### SUP-28 — Conventional Commits Should Be Used

Commit messages should follow a simple Conventional Commit style.

Examples:

- `docs: write initial project vision`
- `docs: define initial user goals`
- `docs: create initial use case model`

#### Rationale

This makes the project history easier to understand.

## AI Collaboration Requirements

### SUP-29 — AI Is a Support Tool, Not the Authority

AI may be used to support analysis, drafting, review, and alternative exploration.

Final decisions remain human decisions.

#### Rationale

The project should reflect the owner's understanding and judgment.

---

### SUP-30 — AI-Generated Content Must Be Reviewed

Any AI-supported artifact should be reviewed, adjusted when necessary, and understood before being accepted.

#### Rationale

The project is intended to build real learning and professional evidence.

## Legal and Ethical Considerations

### SUP-31 — Child-Related Content Requires Care

Because KUNNA relates to children, rights, and caregiving, content should be handled responsibly.

#### Rationale

The product domain has ethical sensitivity.

---

### SUP-32 — No Legal Advice Claim

KUNNA should not present itself as a formal legal advice tool.

#### Rationale

Children's rights content may involve legal concepts, but the product should be careful about its claims and boundaries.

---

### SUP-33 — Colombian Context Should Be Treated Carefully

If Colombian domain context is used, it should be researched and cited properly in content work.

#### Rationale

Domain-specific claims should be accurate and responsible.

## Architecture Questions for Elaboration

Several architecture-related concerns remain unresolved:

- What execution boundary is sufficient for the selected I2 vertical slice.
- Whether the selected behavior requires persistence or can initially remain in memory.
- Whether authentication is required by the selected behavior.
- How content needed by the selected slice should be represented or supplied.
- Whether external files, audio, downloads, or services are relevant to the selected use case.
- Which quality attributes materially influence the architecture hypothesis.

Not every question must be resolved during I2.

Only decisions relevant to the selected use case, current risks, and validation strategy should be addressed.

Significant architecture decisions may be recorded through the Decision Journal or a dedicated ADR when warranted.

## Not Currently Assumed for I2

The following capabilities or technical mechanisms are not automatically required during I2:

- Production-ready backend.
- Mandatory Spring Boot API.
- Production database.
- Authentication.
- Password recovery.
- User registration.
- Admin dashboard.
- Production content management system.
- Mobile application.
- Production deployment.
- Final UI redesign.
- Production-scale infrastructure.

Any of these may be reconsidered if the selected use case or architecture validation strategy provides a concrete justification.

Real legal or sensitive domain content validation also remains a separate evidence requirement and must not be fabricated merely to support implementation.

## Initial Quality Attribute Summary

| Quality Attribute | Current Baseline Expectation                                                                            | Priority |
| ----------------- | ------------------------------------------------------------------------------------------------------- | -------- |
| Usability         | The product should be easy to understand and navigate when relevant to the selected behavior.           | High     |
| Accessibility     | Content should be readable and alternative access methods may be considered when relevant.              | Medium   |
| Reliability       | Implemented behavior should act predictably within the validated slice.                                 | Medium   |
| Security          | Real sensitive personal data is not required for current I2 validation.                                 | High     |
| Performance       | Performance expectations remain preliminary until relevant behavior and architecture needs are clearer. | Medium   |
| Maintainability   | Documentation and code should remain organized and explainable.                                         | High     |
| Traceability      | Relevant requirements, decisions, code, tests, Issues, and Pull Requests should remain connected.       | High     |

These priorities remain provisional baseline values and may be reassessed when the selected I2 use case provides stronger evidence.

## Traceability with Use Cases

| Supplementary Concern    | Related Use Cases                                       |
| ------------------------ | ------------------------------------------------------- |
| Clear language           | View Content, View Daily Tip, Browse Content Categories |
| Simple navigation        | All user-facing use cases                               |
| Search usability         | Search Content                                          |
| Saved content stability  | Bookmark Content, View Saved Content                    |
| Audio accessibility      | Play Audio Content                                      |
| Responsible content      | View Content, View Daily Tip                            |
| Sharing behavior         | Share Content                                           |
| Download behavior        | Download Resource                                       |
| Privacy and profile data | Manage Profile                                          |
| Documentation workflow   | All project artifacts                                   |

This table preserves the initial I1 traceability baseline. It does not indicate which use case will be selected for I2.

## Open Questions

The following questions remain open:

- Which supplementary requirements materially affect the architecturally significant use case selected for I2?
- What minimum quality evidence should be produced by the I2 Java vertical slice?
- Can the selected behavior be validated without persistence?
- Does the selected behavior require authentication?
- How should authoritative content sources be validated when sensitive domain content becomes relevant?
- Which accessibility concerns materially affect the selected behavior?
- Are audio, download, sharing, search, profile, or saved-content capabilities relevant to the selected I2 slice?
- What level of Colombian legal or domain context is necessary for the selected behavior?
- Which architecture assumptions should be validated through executable evidence?

These questions should be narrowed after the architecturally significant use case is selected rather than answered globally in advance.

## Summary

This supplementary specification preserves the initial cross-cutting baseline established during I1 while aligning it with **I2 — Elaboration**.

It complements the use case model by documenting usability, accessibility, language, content, privacy, technical, documentation, AI collaboration, ethical, and architecture-related concerns.

The specification is intentionally provisional.

During I2, only the supplementary requirements that materially affect the selected use case should be refined in greater detail.

The purpose is to support focused analysis, architecture reasoning, executable validation, and traceability without requiring exhaustive upfront specification or predetermined technology choices.
