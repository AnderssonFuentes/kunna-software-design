# 02 — Use Case Model

## Document Purpose

This document defines the use case model baseline for KUNNA.

The model was initially created during the **I1 — Inception Package** and is now reviewed as part of **I2 — Elaboration**.

The purpose of this artifact is to identify candidate actors and use cases that describe how users may interact with KUNNA to achieve user goals.

This document is based on:

- The project vision.
- The user goal baseline.
- The original UX/UI prototype concept.
- Current product and engineering reasoning.

The use cases recorded here are part of the I1 baseline.

They should not all be interpreted as validated requirements, equally important current priorities, or guaranteed implementation commitments.

The I2 baseline review preserves this model while clarifying which assumptions remain provisional before one architecturally significant use case is selected.

## Relationship with Previous Artifacts

The preceding artifacts provide the foundation for this use case model:

| Artifact                | Contribution                                                                      |
| ----------------------- | --------------------------------------------------------------------------------- |
| `README.md`             | Presents the repository and current software engineering direction of KUNNA.      |
| `docs/00-vision.md`     | Defines the product vision baseline, problem hypotheses, target users, and scope. |
| `docs/01-user-goals.md` | Defines candidate user goals and preserves their initial I1 priority baseline.    |

This document connects candidate user goals with candidate system behavior.

The mapping remains refinable as stronger product, domain, and implementation evidence becomes available.

## System Under Design

The system under design is:

**KUNNA**

KUNNA is a digital product concept intended primarily to support mothers, fathers, and caregivers with accessible information related to children's rights, positive parenting, and daily caregiving practices.

The original prototype also explored capabilities such as daily tips, audio content, bookmarks, downloads, search, profiles, and content sharing.

Those capabilities remain candidate product scope rather than guaranteed implementation commitments.

## Current Phase

The project is currently in:

**I2 — Elaboration**

The previous **I1 — Inception Package** milestone was completed and closed.

During I2, the use case model should support focused risk reduction rather than expansion of the complete product scope.

The next major decision is to select one architecturally significant use case and then refine only the behavior, supplementary requirements, domain concepts, system operations, and architecture concerns that materially affect that slice.

This document does not make that selection in advance.

## Scope of the Use Case Model

This model preserves the initial I1 use case baseline while applying only the minimum clarifications needed for I2.

The model is not expected to be complete or final.

Its purpose is to:

- Describe candidate user-system interactions.
- Preserve traceability from user goals.
- Expose assumptions and overlaps.
- Support selection of an architecturally significant use case.
- Provide a basis for focused analysis after selection.

The model focuses on externally observable behavior rather than technical implementation.

Implementation mechanisms should not be modeled as actors unless they represent actual external systems that interact with KUNNA.

## Primary Actor

### Caregiver

The primary actor remains the **Caregiver**.

A caregiver represents a person involved in supporting, protecting, educating, or caring for a child in daily life.

The initial I1 interpretation included:

- Mothers.
- Fathers.
- Relatives.
- Guardians.
- Potentially other caregiving roles.

In Spanish product and domain language:

- Madres.
- Padres.
- Cuidadores.
- Personas responsables del cuidado diario de niñas y niños.

Whether teachers, professionals, institutional users, or other roles belong within the primary audience remains a product question and should not be assumed automatically.

## Candidate Actors

The following actors were identified during I1:

| Actor                     | Type                         | Description                                                             | Initial Priority |
| ------------------------- | ---------------------------- | ----------------------------------------------------------------------- | ---------------- |
| Caregiver                 | Primary actor                | Main user who accesses and interacts with KUNNA behavior.               | High             |
| Guest User                | Provisional actor variant    | Possible user state for accessing behavior without authentication.      | Medium           |
| Registered Caregiver      | Provisional actor variant    | Possible caregiver state with profile, saved content, or preferences.   | Medium           |
| Content Administrator     | Provisional supporting actor | Possible future role responsible for managing content.                  | Low              |
| External Sharing Platform | Provisional external actor   | Possible external system used if sharing requires platform integration. | Low              |

The `Initial Priority` values belong to the I1 baseline and do not define current I2 implementation order.

## Actor Notes

The primary focus remains the **Caregiver**.

The distinction between **Guest User** and **Registered Caregiver** remains provisional.

It depends on whether the selected behavior actually requires:

- Authentication.
- Registration.
- Persistent user identity.
- Saved preferences.
- Profile management.
- Account-specific state.

These concepts should not be introduced simply because they appeared in the original prototype.

`Content Administrator` also remains provisional and should be modeled only if content-management behavior becomes relevant.

`External Sharing Platform` should be treated as an actor only if KUNNA actually integrates with an external system as part of the selected behavior.

Storage, databases, files, repositories, or download mechanisms are implementation concerns unless they represent independently interacting external systems. They should therefore not be treated as actors by default.

## Initial Use Case Baseline

The following use cases were identified during I1:

| ID    | Use Case                  | Primary Actor                    | Related User Goal   | Initial Priority |
| ----- | ------------------------- | -------------------------------- | ------------------- | ---------------- |
| UC-01 | View Content              | Caregiver                        | UG-01, UG-02        | High             |
| UC-02 | View Daily Tip            | Caregiver                        | UG-02, UG-09        | High             |
| UC-03 | Search Content            | Caregiver                        | UG-03               | High             |
| UC-04 | Bookmark Content          | Registered Caregiver / Caregiver | UG-04               | Medium           |
| UC-05 | View Saved Content        | Registered Caregiver / Caregiver | UG-10               | Medium           |
| UC-06 | Play Audio Content        | Caregiver                        | UG-05               | Medium           |
| UC-07 | Download Resource         | Caregiver                        | UG-06               | Medium           |
| UC-08 | Share Content             | Caregiver                        | UG-07               | Medium           |
| UC-09 | Manage Profile            | Registered Caregiver             | UG-08               | Low              |
| UC-10 | Browse Content Categories | Caregiver                        | UG-01, UG-02, UG-09 | High             |

The identifiers, mappings, and priorities above preserve the original I1 baseline.

The `Initial Priority` column should not be interpreted as the current I2 implementation sequence.

Selection for I2 should instead consider:

- Product relevance.
- Risk reduction.
- Architecture significance.
- Requirement uncertainty.
- Domain complexity.
- Ability to produce meaningful executable evidence.

## Use Case Briefs

### UC-01 — View Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to read or consult content related to children's rights, positive parenting, or daily caregiving practices.

**Brief Description:**  
The caregiver selects a relevant content item and accesses its information.

**Related User Goals:**

- UG-01 — Access child rights content.
- UG-02 — Receive positive parenting guidance.

**Initial Priority:** High

**Baseline Note:**

This use case represents a broad content-access interaction and may overlap with more specialized content use cases such as UC-02 and UC-10.

Its boundaries may need refinement if selected for I2.

---

### UC-02 — View Daily Tip

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to discover a short and practical daily tip.

**Brief Description:**  
The caregiver accesses a short content item related to child care, children's rights, or positive parenting when daily-tip behavior is part of the product scope.

**Related User Goals:**

- UG-02 — Receive positive parenting guidance.
- UG-09 — Discover daily tips.

**Initial Priority:** High

**Baseline Note:**

Daily tips originated as a prominent product concept.

Whether a daily tip is a distinct use case or a specialized form of viewing content should be evaluated during later refinement rather than assumed.

---

### UC-03 — Search Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to find content related to a specific topic, situation, or need.

**Brief Description:**  
The caregiver provides search criteria and KUNNA returns relevant content when search behavior is part of the selected product scope.

**Related User Goal:**

- UG-03 — Search for specific topics.

**Initial Priority:** High

**Baseline Note:**

Search remains a candidate capability.

Its current relevance should be evaluated against the selected I2 behavior rather than inferred from its historical High priority.

---

### UC-04 — Bookmark Content

**Primary Actor:** Registered Caregiver / Caregiver

**Goal:** The caregiver wants to save useful content for later consultation.

**Brief Description:**  
The caregiver marks a content item for later access when saved-content behavior is part of the implemented scope.

**Related User Goal:**

- UG-04 — Save useful content.

**Initial Priority:** Medium

**Open Decision:**

It remains unclear whether bookmarking requires authentication, a persistent user identity, local state, or another storage mechanism.

No authentication or persistence solution should be assumed before the selected behavior requires it.

---

### UC-05 — View Saved Content

**Primary Actor:** Registered Caregiver / Caregiver

**Goal:** The caregiver wants to revisit previously saved content.

**Brief Description:**  
The caregiver accesses previously saved content when saved-content behavior is available.

**Related User Goal:**

- UG-10 — Revisit previously saved content.

**Initial Priority:** Medium

**Dependency:**  
This behavior depends conceptually on content having been saved previously.

**Baseline Note:**

UC-04 and UC-05 form a closely related behavioral pair and may require joint refinement if this area becomes relevant to I2.

---

### UC-06 — Play Audio Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to access selected content in audio form.

**Brief Description:**  
The caregiver plays audio-based content when audio is part of the selected product scope.

**Related User Goal:**

- UG-05 — Listen to audio content.

**Initial Priority:** Medium

**Baseline Note:**

Audio originated in the original UX/UI prototype and remains a product hypothesis rather than a guaranteed requirement.

---

### UC-07 — Download Resource

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to retain a useful resource for later use.

**Brief Description:**  
The caregiver requests a downloadable resource when download behavior is part of the selected product scope.

**Related User Goal:**

- UG-06 — Download resources.

**Initial Priority:** Medium

**Baseline Note:**

The use case describes user intent, not the technical mechanism used to store or transfer files.

File systems, storage components, databases, or delivery mechanisms should remain architecture and implementation concerns unless an actual external system interaction must be modeled.

---

### UC-08 — Share Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to share relevant content with another person.

**Brief Description:**  
The caregiver initiates sharing of selected content when sharing behavior is part of the product scope.

**Related User Goal:**

- UG-07 — Share useful content.

**Initial Priority:** Medium

**Open Decision:**

An external sharing platform should be modeled as a supporting actor only if the selected behavior requires an actual integration with an external system.

---

### UC-09 — Manage Profile

**Primary Actor:** Registered Caregiver

**Goal:** The caregiver wants to manage profile information or preferences.

**Brief Description:**  
The caregiver manages relevant profile information if personalization becomes part of the product scope.

**Related User Goal:**

- UG-08 — Manage a basic profile.

**Initial Priority:** Low

**Baseline Note:**

Profile management had Low priority during I1.

Authentication, registration, persistence, account management, and user-profile infrastructure are not automatically required during I2.

---

### UC-10 — Browse Content Categories

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to explore relevant content by category.

**Brief Description:**  
The caregiver browses available content categories when category-based navigation is part of the selected product scope.

**Related User Goals:**

- UG-01 — Access child rights content.
- UG-02 — Receive positive parenting guidance.
- UG-09 — Discover daily tips.

**Initial Priority:** High

**Baseline Note:**

This use case may overlap with UC-01 and UC-02 because all three concern access to content.

Their boundaries should be refined only if one or more become relevant to the selected I2 slice.

## Initial Use Case Priority Groups

The following groups preserve the original I1 priority baseline.

They do **not** define the implementation sequence for I2.

### High Initial Priority

- UC-01 — View Content.
- UC-02 — View Daily Tip.
- UC-03 — Search Content.
- UC-10 — Browse Content Categories.

### Medium Initial Priority

- UC-04 — Bookmark Content.
- UC-05 — View Saved Content.
- UC-06 — Play Audio Content.
- UC-07 — Download Resource.
- UC-08 — Share Content.

### Low Initial Priority

- UC-09 — Manage Profile.

I2 may select a use case from any of these groups if its product relevance, risk profile, or architecture significance justifies doing so.

## Deferred Use Case Hypotheses

The following possible use cases were not prioritized during I1 and are not automatically part of I2:

- Create Account.
- Log In.
- Log Out.
- Recover Password.
- Manage Notifications.
- Receive Push Notifications.
- Create User-Generated Content.
- Manage Content as Administrator.
- Moderate Content.
- Manage Institutional Accounts.
- Configure Advanced Personalization.

These use cases may be reconsidered only when product evidence or selected behavior provides sufficient justification.

## Initial Use Case Relationships

The following behavioral relationships were identified as possible relationships during I1:

| Relationship                                         | Current Interpretation                                            |
| ---------------------------------------------------- | ----------------------------------------------------------------- |
| View Saved Content depends on Bookmark Content       | Saved content must exist before it can be revisited.              |
| Share Content relates to selected content            | Sharing typically operates on content selected by the caregiver.  |
| Download Resource relates to a selected resource     | A resource must be identified before download behavior can occur. |
| Play Audio Content relates to selected audio content | Audio behavior requires content that supports an audio form.      |
| Manage Profile may require user identity             | Profile behavior may depend on a persistent user identity.        |

These statements describe behavioral observations.

They should not automatically be converted into UML `include`, `extend`, generalization, or other formal relationships without additional analysis.

Formal relationships should be introduced only when their semantics are clear and useful.

## Candidate Use Case Diagram — Textual View

The current baseline textual view is:

```text
Caregiver
│
├── View Content
├── View Daily Tip
├── Browse Content Categories
├── Search Content
├── Bookmark Content
├── View Saved Content
├── Play Audio Content
├── Download Resource
└── Share Content

Registered Caregiver
│
└── Manage Profile

External Sharing Platform [provisional]
│
└── May support Share Content if external integration is required
```

`Guest User` and `Registered Caregiver` remain provisional actor variants.

`File Storage / Download Service` is intentionally not represented as an actor in this baseline review because storage is currently an implementation concern, not a confirmed external actor.

## Connection with User Goals

| User Goal                                   | Candidate Use Case         |
| :------------------------------------------ | :------------------------- |
| UG-01 — Access child rights content         | UC-01 — View Content       |
| UG-02 — Receive positive parenting guidance | UC-02 — View Daily Tip     |
| UG-03 — Search for specific topics          | UC-03 — Search Content     |
| UG-04 — Save useful content                 | UC-04 — Bookmark Content   |
| UG-05 — Listen to audio content             | UC-06 — Play Audio Content |
| UG-06 — Download resources                  | UC-07 — Download Resource  |
| UG-07 — Share useful content                | UC-08 — Share Content      |
| UG-08 — Manage a basic profile              | UC-09 — Manage Profile     |
| UG-09 — Discover daily tips                 | UC-02 — View Daily Tip     |
| UG-10 — Revisit previously saved content    | UC-05 — View Saved Content |

This table preserves the initial direct I1 traceability relationship.

Some goals also relate to additional use cases in the broader baseline. For example, UG-01, UG-02, and UG-09 were also associated with UC-10 in the initial use case table.

Those broader mappings should be refined only when they become relevant to selected behavior.

## Initial System Boundary

The current baseline describes user-facing KUNNA behavior such as:

- Viewing relevant content.
- Browsing categories.
- Searching content.
- Viewing daily tips.
- Saving content.
- Revisiting saved content.
- Playing audio content.
- Downloading resources.
- Sharing content.
- Managing a profile.

These behaviors represent candidate product scope.

Their presence in the model does not mean that all belong in the current executable slice.

The system boundary does not currently assume:

- Production-ready backend infrastructure.
- Mandatory authentication.
- Production database persistence.
- Admin dashboard.
- Notification infrastructure.
- Production deployment.
- External API integration.
- Final UI implementation.

Any of these may be introduced if the selected use case or architecture validation strategy demonstrates a concrete need.

## Engineering Value

This use case model supports the project by:

- Connecting candidate user goals with observable system behavior.
- Preserving traceability from the I1 baseline.
- Exposing overlaps and provisional assumptions.
- Supporting selection of an architecturally significant use case.
- Preparing focused domain and system-operation analysis.
- Providing context for selective UML when it adds value.
- Reducing the risk of implementing prototype capabilities without a clear purpose.
- Supporting traceability between requirements, analysis, architecture, code, tests, and evidence.

The use case model should remain lightweight and should evolve only when additional analysis or evidence materially improves it.

## Open Questions

The following questions remain open during I2:

- Which use case is architecturally significant enough to drive the current I2 slice?
- Which user goal does that use case primarily support?
- Which use cases overlap enough to require consolidation or reinterpretation?
- Should UC-01, UC-02, and UC-10 remain distinct behaviors?
- If saved-content behavior becomes relevant, should UC-04 and UC-05 be refined together?
- Does the selected behavior require authentication or persistent user identity?
- Does the selected behavior require persistence?
- Is `Registered Caregiver` necessary as a distinct actor for the selected behavior?
- Is any external supporting actor actually required?
- Which supplementary requirements materially affect the selected use case?
- Which architecture assumptions can be validated through the first executable Java vertical slice?
- Which prototype capabilities should be deferred or discarded?

These questions should be narrowed during `#30` and subsequent I2 work rather than answered globally during the baseline review.

## Current Use Case Model Position

The I1 use case model remains useful as a traceable candidate behavior baseline.

UC-01 through UC-10 are not a mandatory feature list.

Their initial priorities are historical planning inputs rather than the implementation sequence for I2.

The model currently exposes several important areas for later refinement:

- Overlap among content-access use cases.
- Dependence between saving and revisiting content.
- Provisional guest and registered user distinctions.
- Product assumptions inherited from the original prototype.
- Unresolved authentication and persistence needs.
- Unconfirmed external supporting actors.

The next I2 decision is to select one architecturally significant use case.

Only after that selection should the relevant behavior, supplementary requirements, domain model, system operations, and architecture concerns be refined in greater detail.
