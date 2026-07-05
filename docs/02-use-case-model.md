# 02 — Use Case Model

## Document Purpose

This document defines the initial use case model for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to identify the main actors and candidate use cases that describe how users may interact with KUNNA to achieve their goals.

This document is based on:

- The project vision.
- The initial user goals.
- The original UX/UI prototype concept.
- The product-first approach of the project.

## Relationship with Previous Artifacts

The previous artifacts define the foundation for this use case model:

| Artifact                | Contribution                                                           |
| ----------------------- | ---------------------------------------------------------------------- |
| `README.md`             | Presents the repository and the software engineering purpose of KUNNA. |
| `docs/00-vision.md`     | Defines the product vision, problem, target users, and scope.          |
| `docs/01-user-goals.md` | Defines what caregivers need to accomplish.                            |

This document transforms user goals into candidate system interactions.

## System Under Design

The system under design is:

**KUNNA**

KUNNA is a digital product intended to support caregivers with accessible content related to children's rights, positive parenting, daily tips, audio content, bookmarks, downloads, search, profile, and content sharing.

## Scope of the Use Case Model

This is an initial use case model for the Inception phase.

At this stage, the model is not expected to be complete or final. Its purpose is to create enough clarity to guide future requirements, domain modeling, and design decisions.

The current model focuses on user-facing interactions, not technical implementation.

## Primary Actor

### Caregiver

The primary actor is the **Caregiver**.

A caregiver is a person responsible for supporting, protecting, educating, or caring for a child in daily life.

This actor may represent:

- Mothers.
- Fathers.
- Relatives.
- Guardians.
- Teachers.
- Other people involved in child care.

In Spanish product/domain language:

- Madres.
- Padres.
- Cuidadores.
- Personas responsables del cuidado diario de niñas y niños.

## Candidate Actors

| Actor                           | Type                      | Description                                                          | Current Priority |
| ------------------------------- | ------------------------- | -------------------------------------------------------------------- | ---------------- |
| Caregiver                       | Primary actor             | Main user who accesses and interacts with KUNNA content.             | High             |
| Guest User                      | Primary actor variant     | A user who accesses public content without authentication.           | Medium           |
| Registered Caregiver            | Primary actor variant     | A caregiver with a profile, saved content, and possible preferences. | Medium           |
| Content Administrator           | Supporting / future actor | A role that may manage content in future phases.                     | Low              |
| External Sharing Platform       | Supporting actor          | External service or platform used when sharing content.              | Low              |
| File Storage / Download Service | Supporting actor          | Possible external or internal mechanism for downloaded resources.    | Low              |

## Actor Notes

For the first use case model, the main focus is the **Caregiver**.

The distinction between **Guest User** and **Registered Caregiver** is not final yet. It will depend on later decisions about authentication, saved content, profile management, and implementation scope.

## Initial Use Cases

The following use cases are candidates for KUNNA's initial model.

| ID    | Use Case                  | Primary Actor                    | Related User Goal   | Priority |
| ----- | ------------------------- | -------------------------------- | ------------------- | -------- |
| UC-01 | View Content              | Caregiver                        | UG-01, UG-02        | High     |
| UC-02 | View Daily Tip            | Caregiver                        | UG-02, UG-09        | High     |
| UC-03 | Search Content            | Caregiver                        | UG-03               | High     |
| UC-04 | Bookmark Content          | Registered Caregiver / Caregiver | UG-04               | Medium   |
| UC-05 | View Saved Content        | Registered Caregiver / Caregiver | UG-10               | Medium   |
| UC-06 | Play Audio Content        | Caregiver                        | UG-05               | Medium   |
| UC-07 | Download Resource         | Caregiver                        | UG-06               | Medium   |
| UC-08 | Share Content             | Caregiver                        | UG-07               | Medium   |
| UC-09 | Manage Profile            | Registered Caregiver             | UG-08               | Low      |
| UC-10 | Browse Content Categories | Caregiver                        | UG-01, UG-02, UG-09 | High     |

## Use Case Briefs

### UC-01 — View Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to read or consult content related to children's rights, positive parenting, or daily caregiving practices.

**Brief Description:**  
The caregiver opens or selects a content item and views its information in a clear and accessible format.

**Related User Goals:**

- UG-01 — Access child rights content.
- UG-02 — Receive positive parenting guidance.

**Initial Priority:** High

---

### UC-02 — View Daily Tip

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to discover a short and practical daily tip.

**Brief Description:**  
The caregiver accesses a daily tip related to child care, children's rights, or positive parenting.

**Related User Goals:**

- UG-02 — Receive positive parenting guidance.
- UG-09 — Discover daily tips.

**Initial Priority:** High

---

### UC-03 — Search Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to find content about a specific topic.

**Brief Description:**  
The caregiver enters a keyword or topic and the system displays related content results.

**Related User Goal:**

- UG-03 — Search for specific topics.

**Initial Priority:** High

---

### UC-04 — Bookmark Content

**Primary Actor:** Registered Caregiver / Caregiver

**Goal:** The caregiver wants to save useful content for later.

**Brief Description:**  
The caregiver marks a content item as saved or bookmarked.

**Related User Goal:**

- UG-04 — Save useful content.

**Initial Priority:** Medium

**Open Decision:**  
It is not yet clear whether bookmarking requires authentication or whether saved content can exist locally without a user account.

---

### UC-05 — View Saved Content

**Primary Actor:** Registered Caregiver / Caregiver

**Goal:** The caregiver wants to revisit previously saved content.

**Brief Description:**  
The caregiver opens a saved content section and reviews content that was previously bookmarked.

**Related User Goal:**

- UG-10 — Revisit previously saved content.

**Initial Priority:** Medium

**Dependency:**  
This use case depends on the ability to bookmark or save content.

---

### UC-06 — Play Audio Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to listen to content in audio format.

**Brief Description:**  
The caregiver selects an audio item and plays it.

**Related User Goal:**

- UG-05 — Listen to audio content.

**Initial Priority:** Medium

---

### UC-07 — Download Resource

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to download useful resources for later use.

**Brief Description:**  
The caregiver selects a downloadable resource and saves it to their device.

**Related User Goal:**

- UG-06 — Download resources.

**Initial Priority:** Medium

---

### UC-08 — Share Content

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to share useful content with another person.

**Brief Description:**  
The caregiver selects a content item and uses a sharing option to send it through an available channel or external platform.

**Related User Goal:**

- UG-07 — Share useful content.

**Initial Priority:** Medium

---

### UC-09 — Manage Profile

**Primary Actor:** Registered Caregiver

**Goal:** The caregiver wants to manage basic profile information or preferences.

**Brief Description:**  
The caregiver accesses a profile section and manages basic information or preferences.

**Related User Goal:**

- UG-08 — Manage a basic profile.

**Initial Priority:** Low

**Open Decision:**  
This use case is not central during the current Inception phase because authentication and profile implementation are out of scope for now.

---

### UC-10 — Browse Content Categories

**Primary Actor:** Caregiver

**Goal:** The caregiver wants to explore available content by category.

**Brief Description:**  
The caregiver browses categories such as children's rights, positive parenting, daily care, audio content, or resources.

**Related User Goals:**

- UG-01 — Access child rights content.
- UG-02 — Receive positive parenting guidance.
- UG-09 — Discover daily tips.

**Initial Priority:** High

## Use Case Priority Groups

### High Priority

These use cases are central to the first understanding of KUNNA:

- UC-01 — View Content.
- UC-02 — View Daily Tip.
- UC-03 — Search Content.
- UC-10 — Browse Content Categories.

### Medium Priority

These use cases support a richer product experience:

- UC-04 — Bookmark Content.
- UC-05 — View Saved Content.
- UC-06 — Play Audio Content.
- UC-07 — Download Resource.
- UC-08 — Share Content.

### Low Priority

These use cases may require additional technical decisions:

- UC-09 — Manage Profile.

## Use Cases Not Prioritized Yet

The following use cases are intentionally not prioritized during the current phase:

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

These use cases may be considered in later phases, but they are not part of the initial Inception focus.

## Initial Use Case Relationships

The following relationships may be explored later in a UML use case diagram:

| Relationship                                          | Possible Interpretation                                    |
| ----------------------------------------------------- | ---------------------------------------------------------- |
| View Saved Content depends on Bookmark Content        | A user needs saved content before revisiting it.           |
| Share Content depends on View Content                 | A user usually views or selects content before sharing it. |
| Download Resource depends on selecting a resource     | A user must choose a downloadable item first.              |
| Play Audio Content depends on selecting audio content | A user must choose audio content before playing it.        |
| Manage Profile may require authentication             | Profile management may depend on a registered user model.  |

These relationships are preliminary and should not be treated as final UML relationships yet.

## Candidate Use Case Diagram — Textual View

The initial textual view of the use case model is:

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

External Sharing Platform
│
└── Supports Share Content

File Storage / Download Service
│
└── Supports Download Resource
```

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

## Initial System Boundary

The system boundary includes user-facing KUNNA functionality such as:

- Viewing content.
- Browsing categories.
- Searching content.
- Viewing daily tips.
- Saving content.
- Playing audio content.
- Downloading resources.
- Sharing content.
- Managing a basic profile.

The system boundary does not yet include:

- Production backend implementation.
- Real authentication.
- Database persistence.
- Admin dashboard.
- Notification infrastructure.
- Deployment infrastructure.
- External API integration.

## Engineering Value

This use case model helps the project by:

- Connecting user goals with system behavior.
- Preparing the supplementary specification.
- Supporting future UML diagrams.
- Preparing future system sequence diagrams.
- Avoiding premature coding.
- Creating traceability between product vision, user goals, requirements, and design.

## Open Questions

The following questions remain open:

- Should the first implementation focus on content browsing or daily tips?
- Should saved content work without authentication?
- Should the first Java implementation simulate content in memory?
- Which use cases are essential for the first construction iteration?
- Should audio content be modeled before or after text content?
- Should sharing and downloads be implemented early or treated as later features?
- What parts of the original Figma prototype best support the high-priority use cases?

## Summary

This initial use case model identifies the first candidate interactions between caregivers and KUNNA.

The strongest initial use cases are:

- View Content.
- View Daily Tip.
- Search Content.
- Browse Content Categories.

These use cases will guide future requirements, supplementary specifications, UML modeling, and object-oriented design work.
