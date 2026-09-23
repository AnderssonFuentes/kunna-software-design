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

The I2 baseline review preserves this model while clarifying provisional assumptions and recording the architecturally significant use case selected during Issue `#30`.

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

Issue `#30` selects **UC-01 — View Content** as the architecturally significant use case for the first I2 increment.

The next analysis work should refine only the behavior, supplementary requirements, domain concepts, system operations, and architecture concerns that materially affect that slice.

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

## I2 Architecturally Significant Use Case Selection Criteria

Before one use case is selected to drive the first executable increment of I2, a limited set of existing KUNNA use cases will be evaluated using criteria defined in advance.

The purpose of defining these criteria before the selection is to reduce confirmation bias and avoid justifying a preferred use case retrospectively.

The evaluation criteria are:

| Criterion                  | Evaluation Question                                                                                                                                                                                |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| User Value                 | Does the behavior directly support a meaningful caregiver outcome that is consistent with the current KUNNA vision and user goals?                                                                 |
| Domain Learning            | Does the behavior expose useful domain concepts, rules, uncertainties, or content concerns related to children's rights, positive parenting, or caregiving?                                        |
| Architectural Significance | Does the behavior exercise meaningful system responsibilities or boundaries and help reveal architecture concerns without requiring unjustified infrastructure?                                    |
| Risk Reduction             | Can the behavior materially reduce one or more important active I2 product, domain, technical, learning, or process risks?                                                                         |
| Implementation Feasibility | Can the behavior be constrained to a small, responsible, and executable vertical slice within I2 without expanding into unnecessary product scope?                                                 |
| Testability                | Can the behavior produce observable outcomes that can be verified through clear acceptance conditions and meaningful automated tests?                                                              |
| Portfolio Evidence         | Can the resulting work demonstrate credible and explainable software engineering reasoning, traceability, implementation, and testing without allowing portfolio value to determine product scope? |

### Selection Rules

The following rules govern how the criteria will be applied:

- Candidates must already exist in the current KUNNA use case model and be traceable to the existing product baseline or backlog. Issue `#30` should not invent a new product requirement merely to create an attractive implementation candidate.
- Only a limited set of relevant candidates should be compared in depth.
- Historical I1 priority does not determine the I2 selection.
- A use case should not be selected only because it appears easy to implement, visually attractive, technically familiar, or convenient for demonstrating a particular technology.
- Portfolio evidence is a supporting criterion. It must not override user value, product reasoning, domain learning, risk reduction, or responsible engineering scope.
- The comparison should remain qualitative unless stronger evidence justifies quantitative scoring. Arbitrary weighted scores should not create false precision.
- The preferred candidate should provide a useful balance of user value, domain learning, architectural significance, risk reduction, feasibility, and testability.
- Selection of a use case must not preselect a framework, database, persistence mechanism, interface technology, deployment platform, or architecture style.
- The selected use case will receive an initial scope boundary sufficient to guide focused refinement in `#31`, while detailed scenarios, supplementary requirements, domain concepts, system operations, and architecture decisions remain subsequent work.

These criteria established the decision framework before the use case selection was made.

The resulting decision is recorded below after the qualitative comparison.

## I2 Candidate Set and Qualitative Comparison

A limited candidate set is used for deeper comparison so that Issue `#30` can make a focused decision without treating all I1 use cases as equally relevant to the first Elaboration increment.

The candidates are:

- UC-01 — View Content.
- UC-02 — View Daily Tip.
- UC-03 — Search Content.
- UC-04 — Bookmark Content.
- UC-10 — Browse Content Categories.

These candidates already exist in the I1 use case baseline and are traceable to current backlog capabilities:

| Use Case                          | Existing Backlog Capability                                              |
| --------------------------------- | ------------------------------------------------------------------------ |
| UC-01 — View Content              | `KUNNA-PB-020 — View the details of a selected content item`             |
| UC-02 — View Daily Tip            | `KUNNA-PB-026 — Present daily parenting tips`                            |
| UC-03 — Search Content            | `KUNNA-PB-019 — Search and filter available content`                     |
| UC-04 — Bookmark Content          | `KUNNA-PB-021 — Bookmark useful content`                                 |
| UC-10 — Browse Content Categories | `KUNNA-PB-018 — Browse children's rights and positive-parenting content` |

The remaining I1 use cases are not discarded. They are not compared in equal depth for this decision because they currently provide less direct leverage for the first I2 experiment or introduce dependencies that are better evaluated later:

- UC-05 — View Saved Content depends conceptually on previously saved content and is therefore closely coupled to UC-04.
- UC-06 — Play Audio Content remains a prototype-derived product hypothesis and alternative content format.
- UC-07 — Download Resource can introduce delivery, storage, or file-handling concerns before those mechanisms are justified.
- UC-08 — Share Content may introduce external integration concerns before sharing is sufficiently justified.
- UC-09 — Manage Profile can introduce identity, authentication, persistence, and personal-data concerns before the selected behavior demonstrates a need for them.

### Qualitative Comparison

The comparison below applies the criteria defined above without numerical weighting.

| Candidate                         | User Value                                                                                                                                         | Domain Learning                                                                                                                            | Architectural Significance                                                                                                                                                          | Risk Reduction                                                                                                                                                                                                                                                          | Implementation Feasibility                                                                                                                         | Testability                                                                                        | Portfolio Evidence                                                                                                                                                     |
| --------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| UC-01 — View Content              | Directly supports the core KUNNA purpose through UG-01 and UG-02 by enabling caregivers to access child-rights and positive-parenting information. | Exposes content meaning, credibility, provenance, and caregiver-oriented information in the core product domain.                           | Exercises meaningful content-access responsibilities and boundaries without inherently requiring authentication, persistence, external integration, or a production interface.      | Strongly relevant to R01, R03, R08, R09, R10, and R13 because it can constrain the first slice, challenge prototype assumptions, keep infrastructure minimal, expose sensitive-content provenance, preserve traceability, and provide executable architecture evidence. | Can be constrained to one focused content-access flow while deferring search, categories, bookmarks, profiles, and other surrounding capabilities. | Selection and access outcomes can be verified through clear behavior examples and automated tests. | Can demonstrate end-to-end traceability from vision and goals through analysis, implementation, and tests without requiring technology-driven scope.                   |
| UC-02 — View Daily Tip            | Supports practical guidance through UG-02 and UG-09, but daily tips remain an unvalidated product hypothesis inherited from the original concept.  | Exposes caregiving-content concerns, although much of the domain learning overlaps with the broader content-access behavior of UC-01.      | May be architecturally meaningful if daily-tip behavior has distinct rules, but it may instead prove to be a specialized form of viewing content.                                   | Relevant to R03 and R09, while premature selection could also preserve a prototype-derived assumption that has not yet been validated.                                                                                                                                  | Relatively easy to constrain to a small slice.                                                                                                     | Short-tip access behavior can be verified clearly.                                                 | Can produce useful evidence, but may provide less architectural learning if later refinement collapses it into UC-01.                                                  |
| UC-03 — Search Content            | Supports UG-03 and the candidate need to find relevant information efficiently.                                                                    | Can reveal topic, relevance, and content-classification concepts, but attention may shift quickly from the domain toward search mechanics. | Introduces query and retrieval responsibilities, while also creating a risk of prematurely selecting search, indexing, persistence, or infrastructure mechanisms.                   | Relevant to R03, R08, R10, and R13 because it can challenge prototype assumptions and exercise executable boundaries, but it can also increase technical scope prematurely.                                                                                             | Feasible if search behavior and the searchable content set are tightly constrained; otherwise scope can expand quickly.                            | Search criteria and returned results can be tested deterministically.                              | Can demonstrate clear technical behavior and automated tests, but technical attractiveness must not become the reason for selection.                                   |
| UC-04 — Bookmark Content          | Supports UG-04 and the need to return to useful information later, although bookmarking is one possible solution to that broader need.             | Provides learning about saved state and continuity of use, with less direct exposure to KUNNA's core sensitive-content domain than UC-01.  | Strongly exposes questions about state, identity, persistence, and system boundaries.                                                                                               | Relevant especially to R08, R10, R13, and R14, but selecting it may also introduce persistence, identity, or privacy concerns earlier than necessary.                                                                                                                   | Feasible only if the slice avoids assuming authentication, databases, or production persistence before they are justified.                         | Bookmarking behavior can be expressed with clear state transitions and automated verification.     | Can demonstrate meaningful state-oriented design and testing, but has a higher risk of becoming infrastructure-driven.                                                 |
| UC-10 — Browse Content Categories | Supports content access and discovery and is associated with UG-01, UG-02, and UG-09.                                                              | Can expose content taxonomy, categorization, and relationships among caregiver-oriented information.                                       | Exercises organization and navigation responsibilities, but substantially overlaps with UC-01 and UC-02 and may remain closer to navigation structure than an architectural driver. | Relevant to R01, R03, and R10 because it forces clarification of overlapping content-access behavior and preserves traceability.                                                                                                                                        | Can be constrained to a narrow slice without requiring authentication or persistence.                                                              | Category exploration and resulting content can be verified clearly.                                | Can provide useful traceability and implementation evidence, though it may expose less architectural tension than candidates involving core content handling or state. |

### Comparison Position

The comparison intentionally does not produce a numerical score or automatic winner.

At this point:

- UC-01 has the strongest direct connection to KUNNA's core product purpose and sensitive-content domain while remaining technically constrainable.
- UC-02 is focused and feasible but may be a specialization of UC-01 rather than a distinct architectural driver.
- UC-03 is clearly testable and technically meaningful but may shift I2 toward search mechanics before search is sufficiently justified.
- UC-04 exposes substantial architectural uncertainty around state, persistence, identity, and privacy, but may introduce those concerns before they are needed for the core product behavior.
- UC-10 supports product discovery and domain organization but overlaps materially with UC-01 and UC-02.

The final selection is recorded in the next section with its rationale, risk mapping, treatment of non-selected alternatives, and initial scope boundary.

No framework, database, interface technology, persistence mechanism, deployment platform, or architecture style is selected by this comparison.

## Selected Architecturally Significant Use Case

**Selected Use Case:** UC-01 — View Content

**Primary Actor:** Caregiver

**Related User Goals:**

- UG-01 — Access child rights content.
- UG-02 — Receive positive parenting guidance.

**Related Backlog Capability:**

- `KUNNA-PB-020 — View the details of a selected content item`.

### Decision Rationale

UC-01 — View Content is selected as the architecturally significant use case for the first I2 increment because it provides the strongest current balance of user value, domain learning, architectural significance, risk reduction, implementation feasibility, testability, and credible engineering evidence.

The selection is not based on historical I1 priority, visual prominence in the original prototype, ease of implementation, or the attractiveness of a particular technology.

UC-01 connects directly to the core KUNNA product direction: enabling caregivers to consult accessible information about children's rights, positive parenting, and daily caregiving practices.

It also exposes one of the most important domain concerns in the project: content credibility and provenance. This makes the slice useful for learning about the actual KUNNA domain rather than primarily exercising a secondary interaction mechanism.

From an architectural perspective, UC-01 is significant enough to exercise meaningful responsibilities and boundaries for obtaining and presenting a selected content item, while still allowing I2 to defer authentication, persistence, external integrations, production infrastructure, and final interface technology unless later evidence demonstrates a concrete need.

The use case is also sufficiently small to support a focused executable Java vertical slice with automated tests, allowing the project to evaluate architecture through behavior rather than through documentation alone.

### Risk Reduction Expected from the Selection

The selection is expected to reduce or provide evidence against the following risks:

| Risk Area                      | Relevant Risks | Expected Contribution                                                                                                                                                                              |
| ------------------------------ | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Product                        | R01, R03       | Constrains I2 to one core product slice and avoids reproducing multiple prototype-derived capabilities without justification.                                                                      |
| Domain                         | R09            | Forces explicit treatment of content provenance, credibility, and responsible handling for child-, caregiver-, and rights-related information.                                                     |
| Technical / Architecture       | R08, R13       | Allows a meaningful executable slice without preselecting frameworks or infrastructure and provides evidence for later architecture validation.                                                    |
| Traceability / Process         | R10            | Creates a direct path from vision and user goals through selected behavior, requirements, analysis, code, tests, and validation evidence.                                                          |
| Learning / Engineering Process | R04, R05       | Requires the project owner to understand and verify the selected behavior while ensuring implementation begins only after enough slice-specific analysis exists to make the experiment meaningful. |

Other active risks remain relevant to I2 but are not primary reasons for selecting UC-01.

In particular, R14 — privacy remains active but is not expected to drive the first slice because UC-01 does not currently require personal data, authentication, or persistent user identity.

R15 — requirements quality will be addressed in `#31` by refining only the supplementary requirements that materially affect UC-01.

### Initial Scope Boundary

The initial scope boundary is intentionally narrow.

#### In Scope for the Selected Slice

- A caregiver selects or requests one available KUNNA content item.
- KUNNA provides the selected content item's relevant information for consultation.
- The content belongs to the current KUNNA domain of children's rights, positive parenting, or daily caregiving practices.
- The slice preserves traceability to UG-01 and UG-02.
- Content credibility and provenance are treated as explicit domain and requirement concerns.
- The behavior must be expressible through observable outcomes that can later be automated as tests.
- The slice must be implementable without assuming infrastructure that the behavior does not require.

#### Outside the Initial Scope

The following behaviors remain outside the initial UC-01 slice unless later analysis demonstrates that one is strictly necessary to validate the selected behavior:

- Daily-tip specialization.
- Search or filtering.
- Category browsing.
- Bookmarking or saved-content behavior.
- Audio playback.
- Downloads.
- Sharing.
- Profile management.
- Registration or authentication.
- Persistent caregiver identity.
- Production database persistence.
- Administrative content-management workflows.
- External integrations.
- Production deployment.
- Final user-interface implementation.

Content provenance and validation are relevant to the selected slice, but Issue `#30` does not define a complete editorial, legal, clinical, psychological, or content-governance workflow.

### Non-Selected Alternatives

The other deeply compared candidates remain part of the product baseline but are not prioritized for the first I2 increment:

- **UC-02 — View Daily Tip:** not selected because daily-tip behavior remains a prototype-derived hypothesis and may later prove to be a specialization of UC-01 rather than a distinct architectural driver.
- **UC-03 — Search Content:** not selected because search is currently a supporting discovery capability and could shift early I2 work toward search mechanics or infrastructure before the core content behavior is sufficiently understood.
- **UC-04 — Bookmark Content:** not selected because its architectural value comes largely from state, identity, persistence, and privacy concerns that are not yet necessary to exercise the core KUNNA product behavior.
- **UC-10 — Browse Content Categories:** not selected because it overlaps materially with UC-01 and UC-02 and currently appears more useful as a navigation or content-organization concern than as the primary architectural driver.

These alternatives are deferred, not rejected.

They may be reconsidered when product evidence, the selected slice, or later iteration learning provides stronger justification.

### Technology and Architecture Boundary

This selection does **not** choose:

- A framework.
- Spring Boot.
- An API style.
- A database.
- A persistence mechanism.
- Authentication technology.
- A frontend framework.
- A final interface technology.
- A deployment platform.
- A specific architecture style.

Those decisions remain subject to later analysis and architecture validation.

### Handoff to Issue #31

Issue `#31` should use UC-01 as its focused input.

The next work should refine only:

- The behavior and scenarios necessary to understand UC-01.
- Supplementary requirements that materially affect UC-01.
- Content-provenance and quality concerns relevant to the selected slice.
- Assumptions and open questions that must be resolved before focused domain and system-operation analysis.

Issue `#31` should not expand the selection into a complete product specification or prematurely define the final architecture.

## Open Questions

The following questions remain open after the Issue `#30` selection:

- Which UC-01 scenarios are necessary for the first executable slice?
- Which content concepts and rules are required to represent the selected behavior meaningfully?
- Which content-provenance requirements are necessary for responsible validation of the slice?
- Which supplementary requirements materially affect UC-01?
- Which system operations are needed to express the selected behavior?
- Which architecture assumptions should be tested through the first executable Java vertical slice?
- Does any requirement discovered during refinement create a justified need for persistence, an external actor, or another technical mechanism?
- How should the overlap among UC-01, UC-02, and UC-10 be refined without expanding the first slice?

These questions should be addressed selectively during `#31`, `#32`, and subsequent I2 work rather than answered globally.

## Current Use Case Model Position

The I1 use case model remains useful as a traceable candidate behavior baseline.

UC-01 through UC-10 are not a mandatory feature list.

Their initial priorities remain historical planning inputs rather than the implementation sequence for I2.

Issue `#30` selects **UC-01 — View Content** as the architecturally significant use case for the first I2 increment.

The selection narrows the immediate product and engineering focus without discarding the remaining candidate use cases.

The model still exposes areas that may require later refinement:

- Overlap among UC-01, UC-02, and UC-10.
- Dependence between saving and revisiting content.
- Provisional guest and registered user distinctions.
- Product assumptions inherited from the original prototype.
- Unresolved authentication and persistence needs outside the selected slice.
- Unconfirmed external supporting actors.

The next I2 step is `#31 — Refine the selected use case and relevant supplementary requirements`.

Only UC-01 behavior and requirements that materially affect the selected slice should be refined at that stage.
