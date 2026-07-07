# 03 — Supplementary Specification

## Document Purpose

This document defines the initial supplementary specification for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to document requirements, constraints, quality attributes, and general rules that are not fully described by individual use cases.

This document complements:

- `README.md`
- `docs/00-vision.md`
- `docs/01-user-goals.md`
- `docs/02-use-case-model.md`

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
- Future implementation assumptions.

## System Under Design

The system under design is:

**KUNNA**

KUNNA is a digital product intended to support caregivers with accessible content related to children's rights, positive parenting, daily tips, audio content, bookmarks, downloads, search, profile, and content sharing.

## Current Phase

The project is currently in:

**I1 — Inception Package**

During this phase, the main objective is not to implement production code.

The objective is to clarify:

- Product vision.
- User goals.
- Use cases.
- Supplementary requirements.
- Glossary.
- Risks.
- Development plan.
- Development framework.
- AI collaboration policy.
- Decision records.
- Product backlog.

## Scope of This Specification

This document defines initial supplementary requirements for the project.

At this stage, the requirements are not final. They provide a starting point for future elaboration, design, and implementation.

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

## Usability Requirements

### SUP-01 — Clear and Accessible Language

KUNNA should use clear, simple, and understandable language for caregivers.

Product and domain content should avoid unnecessary legal, technical, or academic complexity.

#### Rationale

The product is intended for mothers, fathers, and caregivers who may need practical guidance in daily situations.

---

### SUP-02 — Simple Navigation

KUNNA should provide simple navigation between content, categories, daily tips, saved content, audio, downloads, search, profile, and sharing options.

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

Future content sources should be reviewed carefully.

#### Rationale

The product domain involves children, care, and rights. Inaccurate content could be harmful.

---

### SUP-12 — Content Should Be Organized by Topics or Categories

Content should be organized in a way that supports browsing and searching.

Possible initial categories may include:

- Derechos de niñas y niños.
- Crianza positiva.
- Cuidado diario.
- Tips diarios.
- Recursos.
- Audio content.

---

### SUP-13 — Content Should Support Reuse

Useful content should be easy to save, revisit, share, or download when appropriate.

#### Rationale

Caregivers may need to return to important content later.

## Security and Privacy Requirements

### SUP-14 — No Sensitive Data in Early Phases

During the current phase, the project should avoid collecting or implementing real personal data.

#### Rationale

The current focus is documentation, analysis, and design. Authentication and real user data are out of scope for now.

---

### SUP-15 — Future Profile Data Must Be Treated Carefully

If user profiles are implemented in a future phase, profile data should be handled with privacy and security considerations.

#### Rationale

The product may eventually include saved content, preferences, or user information.

---

### SUP-16 — Authentication Is Out of Scope for Inception

Authentication, password recovery, and account management are not part of the current Inception implementation scope.

#### Rationale

These features require technical and security decisions that should be addressed in later phases.

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

Future implementations should prioritize fast access to content, search results, and daily tips.

#### Rationale

Caregivers may need quick consultation.

---

### SUP-20 — Performance Requirements Are Preliminary

Exact performance targets are not defined during Inception.

#### Rationale

The project has not yet entered construction, architecture, or deployment decisions.

## Technical Constraints

### SUP-21 — No Production Code During Inception

Production code is intentionally out of scope during the current phase.

#### Rationale

The project follows a documentation-first and product-first approach.

---

### SUP-22 — Future Implementation Should Be Progressive

Future implementation should start with simple Java concepts before moving to advanced architecture or Spring Boot.

#### Rationale

The project is also a learning path for software engineering, Java, object-oriented design, and backend development.

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

Any AI-supported artifact should be reviewed, adjusted, and understood before being accepted.

#### Rationale

The project is intended to build real learning and professional evidence.

## Legal and Ethical Considerations

### SUP-31 — Child-Related Content Requires Care

Because KUNNA relates to children, rights, and caregiving, content should be handled responsibly.

#### Rationale

The product domain has ethical sensitivity.

---

### SUP-32 — No Legal Advice Claim

KUNNA should not present itself as a formal legal advice tool during early phases.

#### Rationale

Children's rights content may involve legal concepts, but the product should be careful about its claims.

---

### SUP-33 — Colombian Context Should Be Treated Carefully

If Colombian domain context is used, it should be researched and cited properly in future content work.

#### Rationale

Domain-specific claims should be accurate and responsible.

## Future Architecture Considerations

The following architecture-related concerns are not resolved yet:

- Whether the first implementation will be a console Java application, desktop simulation, web prototype, or API.
- Whether saved content will be stored in memory, file storage, local database, or backend database.
- Whether authentication will be required for bookmarks.
- Whether content will be static, local, or managed through an admin interface.
- Whether audio files will be local assets or remote resources.
- Whether downloads will be simulated or implemented with real file handling.

These concerns should be addressed in future decision records or development planning documents.

## Out of Scope for This Phase

The following items are out of scope during the current Inception phase:

- Production backend.
- Spring Boot API.
- Real database implementation.
- Authentication.
- Password recovery.
- User registration.
- Admin dashboard.
- Real content management system.
- Mobile app implementation.
- Deployment.
- Final UI redesign.
- Real legal content validation.

## Initial Quality Attribute Summary

| Quality Attribute | Initial Expectation                                                          | Priority |
| ----------------- | ---------------------------------------------------------------------------- | -------- |
| Usability         | The product should be easy to understand and navigate.                       | High     |
| Accessibility     | Content should be readable and audio may support access.                     | Medium   |
| Reliability       | Content and saved items should behave predictably in future implementations. | Medium   |
| Security          | Real personal data is out of scope during Inception.                         | High     |
| Performance       | Content access should feel fast in future implementations.                   | Medium   |
| Maintainability   | Documentation and code should remain organized and explainable.              | High     |
| Traceability      | Artifacts should connect to Issues, PRs, and milestones.                     | High     |

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

## Open Questions

The following questions remain open:

- What minimum quality requirements should be applied to the first Java implementation?
- Should the first Java version simulate content without persistence?
- Should bookmarks require authentication in the future?
- How should content sources be validated?
- What accessibility requirements should be prioritized first?
- Should audio content be part of the first construction iteration?
- Should downloads be implemented or simulated initially?
- What level of Colombian legal/domain context should be included in early versions?

## Summary

This supplementary specification defines initial cross-cutting requirements and constraints for KUNNA.

It complements the use case model by documenting usability, accessibility, language, content, privacy, technical, documentation, AI collaboration, ethical, and future architecture considerations.

The main purpose is to avoid premature coding and provide a stronger foundation for future analysis, design, and implementation.
