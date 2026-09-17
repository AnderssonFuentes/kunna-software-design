# 01 — User Goals

## Document Purpose

This document defines the user goal baseline for KUNNA.

The user goals were initially established during the **I1 — Inception Package** and are now reviewed as part of **I2 — Elaboration**.

The purpose of this artifact is to identify what users may need to achieve before detailed system behavior, design, or implementation decisions are committed.

User goals connect the product vision with use cases, requirements, analysis, and implementation evidence.

The goals recorded here originated as an initial product baseline.

They should not all be interpreted as validated user needs, equally important current priorities, or guaranteed implementation commitments.

## Relationship with the Vision Document

The project vision defines what KUNNA is intended to become, why it exists, who it may serve, and which product assumptions remain provisional.

This document focuses on user intent by asking:

- What may caregivers need to accomplish?
- Which outcomes could be valuable for them?
- Which user intentions should guide use-case reasoning?
- What behavior might the system need to support?

The answers remain subject to refinement as stronger product evidence becomes available.

## Target Users

The candidate primary users identified during I1 are:

- Mothers.
- Fathers.
- Caregivers.
- People responsible for the daily care and protection of children.

In Spanish product and domain language:

- Madres.
- Padres.
- Cuidadores.
- Personas responsables del cuidado diario de niñas y niños.

The exact boundaries of the target audience remain provisional.

The project should not broaden the primary audience without product evidence that justifies doing so.

## Primary User Role

For the current baseline, the main user role is:

**Caregiver**

A caregiver represents a person involved in supporting, protecting, educating, or caring for a child in daily life.

During I1, this role was used as an umbrella concept that could include mothers, fathers, relatives, guardians, and potentially other caregiving roles.

Whether teachers, professionals, institutional users, or other roles belong within the primary KUNNA audience remains an open product question and should not be assumed automatically.

## User Context

The current product hypothesis is that caregivers may need guidance while dealing with real-life parenting or caregiving situations.

They may value information that is:

- Clear.
- Practical.
- Trustworthy.
- Easy to revisit.
- Easy to understand.
- Available in appropriate formats.
- Connected to daily caregiving needs.

KUNNA should avoid assuming that users have technical, legal, or specialized knowledge.

These statements represent the current product baseline rather than completed user research.

## Initial User Goal Baseline

The following goals were identified during I1 as candidate outcomes caregivers may want to achieve when using KUNNA.

| ID    | User Goal                           | Description                                                                                           | Initial Priority |
| ----- | ----------------------------------- | ----------------------------------------------------------------------------------------------------- | ---------------- |
| UG-01 | Access child rights content         | The caregiver wants to understand content related to children's rights in a clear and accessible way. | High             |
| UG-02 | Receive positive parenting guidance | The caregiver wants to access practical tips about positive parenting and daily care.                 | High             |
| UG-03 | Search for specific topics          | The caregiver wants to find information about a specific topic, situation, or need.                   | High             |
| UG-04 | Save useful content                 | The caregiver wants to bookmark content to revisit it later.                                          | Medium           |
| UG-05 | Listen to audio content             | The caregiver wants to consume selected content in audio format.                                      | Medium           |
| UG-06 | Download resources                  | The caregiver wants to download useful materials or resources for later use.                          | Medium           |
| UG-07 | Share useful content                | The caregiver wants to share relevant information with another person.                                | Medium           |
| UG-08 | Manage a basic profile              | The caregiver wants to manage basic personal preferences or profile information.                      | Low              |
| UG-09 | Discover daily tips                 | The caregiver wants to receive or browse short daily tips related to care, rights, or parenting.      | High             |
| UG-10 | Revisit previously saved content    | The caregiver wants to return to content that was previously saved or marked as useful.               | Medium           |

The `Initial Priority` values are part of the I1 baseline.

They should not be interpreted as the current I2 implementation order or as validated product priorities.

I2 should select and refine behavior based on current risk, product reasoning, architecture significance, and available evidence rather than automatically following this table.

## High-Level User Goals

The initial high-level goal groups are:

1. Understand children's rights.
2. Learn positive parenting practices.
3. Find practical information efficiently.
4. Save and revisit useful content when that behavior is justified.
5. Access content through appropriate formats.
6. Share relevant information when useful.
7. Support a personalized experience only when product evidence requires it.

These groups summarize the I1 baseline and may overlap.

They should not be interpreted as a final decomposition of the product.

## Goal Details

### UG-01 — Access child rights content

**As a caregiver**, I want to access clear content about children's rights, so that I can better understand how to protect and support children.

#### Expected Outcome

The caregiver can consult information about children's rights without needing specialized legal knowledge.

#### Notes

This goal is central to the initial KUNNA product concept.

Any authoritative or user-facing child-rights content requires appropriate source provenance and validation.

---

### UG-02 — Receive positive parenting guidance

**As a caregiver**, I want to access practical guidance about positive parenting, so that I can improve daily caregiving practices.

#### Expected Outcome

The caregiver receives useful and understandable information related to parenting, care, communication, and child protection.

#### Notes

This goal connects the product concept with daily caregiving situations.

The exact form of the guidance remains subject to product and content validation.

---

### UG-03 — Search for specific topics

**As a caregiver**, I want to search for a specific topic, so that I can quickly find relevant content when I need it.

#### Expected Outcome

The caregiver can locate content related to a topic, situation, or need.

#### Notes

Search remains a candidate capability.

Its I2 priority should be determined only if the selected use case or product evidence makes search relevant.

---

### UG-04 — Save useful content

**As a caregiver**, I want to save useful content, so that I can revisit it later.

#### Expected Outcome

The caregiver can mark content for later consultation when saved-content behavior is part of the implemented scope.

#### Notes

This goal supports continuity and repeated consultation.

It overlaps with UG-10 and may later be refined together with the related use cases.

---

### UG-05 — Listen to audio content

**As a caregiver**, I want to listen to selected content, so that I can consume information in an alternative format.

#### Expected Outcome

The caregiver can access audio-based content when audio is justified by the selected product behavior.

#### Notes

Audio originated as a capability in the original UX/UI prototype.

It remains a product hypothesis rather than a guaranteed requirement.

---

### UG-06 — Download resources

**As a caregiver**, I want to download useful resources, so that I can keep them for later use.

#### Expected Outcome

The caregiver can download selected materials when download behavior is included in the validated product scope.

#### Notes

Downloads may introduce file-format, storage, content-management, and delivery decisions.

The capability should not be implemented merely because it existed in the original prototype.

---

### UG-07 — Share useful content

**As a caregiver**, I want to share useful content with others, so that more people can access relevant information.

#### Expected Outcome

The caregiver can share content when sharing behavior is justified and supported by the selected product scope.

#### Notes

Sharing may support the product's social value, but its priority remains provisional.

---

### UG-08 — Manage a basic profile

**As a caregiver**, I want to manage a basic profile, so that the product can support a more personalized experience.

#### Expected Outcome

The caregiver can manage relevant profile information if personalization becomes part of the product scope.

#### Notes

This goal had **Low** initial priority during I1.

Profiles, authentication, registration, persistence, and account management are not automatically required during I2.

---

### UG-09 — Discover daily tips

**As a caregiver**, I want to discover short daily tips, so that I can receive practical guidance in a simple format.

#### Expected Outcome

The caregiver can access short information related to parenting, rights, or child care when daily-tip behavior is part of the selected product scope.

#### Notes

Daily tips were prominent in the original product concept.

Whether users actively browse them, receive them automatically, or need this capability at all remains to be refined.

No I2 implementation priority is implied by the initial High rating.

---

### UG-10 — Revisit previously saved content

**As a caregiver**, I want to return to saved content, so that I can review information that I previously considered useful.

#### Expected Outcome

The caregiver can access previously saved content when saved-content behavior is implemented.

#### Notes

This goal depends on UG-04 and may be refined together with bookmark or saved-content behavior.

The relationship between saving and revisiting content should be clarified if this area is selected for deeper analysis.

## Candidate Actors

The following actors were identified during the initial analysis:

| Actor                 | Description                                                       |
| --------------------- | ----------------------------------------------------------------- |
| Caregiver             | Main user who accesses and interacts with KUNNA content.          |
| Content Administrator | Possible future role responsible for managing content.            |
| Guest User            | Possible user who accesses public content without authentication. |
| Registered User       | Possible user who has a profile and saved preferences.            |

The primary focus remains the **Caregiver**.

`Guest User`, `Registered User`, and `Content Administrator` remain provisional actor hypotheses.

Authentication, registration, administration, and user-state distinctions should not be introduced unless the selected behavior and architecture evidence demonstrate that they are necessary.

## Deferred Goal Hypotheses

The following possible goals were not prioritized during I1 and are not automatically part of I2:

- Creating an account.
- Recovering a password.
- Managing advanced personalization.
- Receiving push notifications.
- Creating user-generated content.
- Managing professional or institutional accounts.
- Administering a full content management system.

These goals may be reconsidered in future work if product evidence or a selected use case provides sufficient justification.

## Relationship with the Use Case Model

The user goals established during I1 informed the initial use case model.

The original goal-to-use-case mapping includes:

| User Goal                           | Candidate Use Case |
| ----------------------------------- | ------------------ |
| Access child rights content         | View Content       |
| Receive positive parenting guidance | View Daily Tip     |
| Search for specific topics          | Search Content     |
| Save useful content                 | Bookmark Content   |
| Listen to audio content             | Play Audio Content |
| Download resources                  | Download Resource  |
| Share useful content                | Share Content      |
| Manage a basic profile              | Manage Profile     |
| Revisit previously saved content    | View Saved Content |

This table preserves the initial I1 traceability relationship.

It does not determine which use case should be selected for I2.

The current use case model may refine, combine, defer, or reinterpret these mappings as analysis progresses.

## Engineering Value

User-goal reasoning helps prevent implementation from becoming detached from user intent.

This document supports the project by:

- Clarifying candidate user outcomes.
- Connecting the product vision with system behavior.
- Supporting use-case analysis.
- Exposing overlaps and assumptions that may require refinement.
- Reducing the risk of implementing prototype features without a clear purpose.
- Supporting traceability between product reasoning and engineering work.

User-goal documentation should remain lightweight and should evolve only when new evidence materially changes the baseline.

## Open Questions

The following questions remain open during I2:

- Which user goal is most relevant to the architecturally significant use case selected for I2?
- Do the initial High/Medium/Low priorities still represent useful product priorities?
- Which goals overlap enough to require consolidation or reinterpretation?
- Does the selected behavior require guest and registered user distinctions?
- Does the selected behavior require authentication or persistence?
- Are audio, downloads, sharing, profiles, search, or saved-content capabilities relevant to the selected I2 slice?
- How should authoritative content sources influence user-goal refinement?
- Which parts of the original UX/UI prototype genuinely support current user outcomes?
- Which assumptions should be deferred or discarded?

These questions should be narrowed after the architecturally significant use case is selected rather than answered globally during the I1 baseline review.

## Current User Goal Position

The I1 user-goal baseline remains useful, but it is provisional.

UG-01 through UG-10 should be treated as traceable product hypotheses rather than a mandatory feature list.

Their initial priorities are historical planning inputs, not the implementation sequence for I2.

The next I2 decision is to select one architecturally significant use case and then refine only the user goals and supplementary requirements that materially affect that slice.
