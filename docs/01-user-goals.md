# 01 — User Goals

## Document Purpose

This document defines the initial user goals for KUNNA as part of the **I1 — Inception Package**.

The purpose of this artifact is to identify what users need to achieve before defining detailed use cases, system behavior, or implementation decisions.

User goals help connect the product vision with future use cases and requirements.

## Relationship with the Vision Document

The project vision defines what KUNNA is, why it exists, and who it serves.

This document takes the next step by asking:

- What do caregivers need to accomplish?
- What outcomes are valuable for them?
- What user intentions should guide the first use case model?
- What should the system help users do?

## Target Users

The initial target users are:

- Mothers.
- Fathers.
- Caregivers.
- People responsible for the daily care and protection of children.

In Spanish product/domain language:

- Madres.
- Padres.
- Cuidadores.
- Personas responsables del cuidado diario de niñas y niños.

## Primary User Role

For the initial analysis, the main user role will be:

**Caregiver**

A caregiver is a person responsible for supporting, protecting, educating, or caring for a child in daily life.

This role may include mothers, fathers, relatives, guardians, teachers, or other people involved in child care.

## User Context

Caregivers may need guidance while dealing with real-life parenting or caregiving situations.

They may want information that is:

- Clear.
- Practical.
- Trustworthy.
- Easy to revisit.
- Easy to understand.
- Available in different formats.
- Connected to daily caregiving needs.

KUNNA should support these needs without assuming that the user has technical, legal, or specialized knowledge.

## Initial User Goals

The following user goals describe what caregivers may want to achieve when using KUNNA.

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

## High-Level User Goals

The initial high-level goals are:

1. Understand children's rights.
2. Learn positive parenting practices.
3. Find practical information quickly.
4. Save and revisit useful content.
5. Consume content in accessible formats.
6. Share relevant information.
7. Build a simple personalized experience.

## Goal Details

### UG-01 — Access child rights content

**As a caregiver**, I want to access clear content about children's rights, so that I can better understand how to protect and support children.

#### Expected Outcome

The caregiver can consult information about children's rights without needing specialized legal knowledge.

#### Notes

This goal is central to KUNNA's product identity.

---

### UG-02 — Receive positive parenting guidance

**As a caregiver**, I want to access practical guidance about positive parenting, so that I can improve daily caregiving practices.

#### Expected Outcome

The caregiver receives useful and understandable tips related to parenting, care, communication, and child protection.

#### Notes

This goal connects the product with daily caregiving situations.

---

### UG-03 — Search for specific topics

**As a caregiver**, I want to search for a specific topic, so that I can quickly find relevant content when I need it.

#### Expected Outcome

The caregiver can enter a topic or keyword and find related content.

#### Notes

Search will likely become an important use case in future iterations.

---

### UG-04 — Save useful content

**As a caregiver**, I want to save useful content, so that I can revisit it later.

#### Expected Outcome

The caregiver can mark content as saved or bookmarked.

#### Notes

This goal supports continuity and repeated consultation.

---

### UG-05 — Listen to audio content

**As a caregiver**, I want to listen to selected content, so that I can consume information in an accessible format.

#### Expected Outcome

The caregiver can play audio-based content related to parenting, rights, or daily tips.

#### Notes

Audio may be useful for caregivers who prefer listening or who cannot read content at a specific moment.

---

### UG-06 — Download resources

**As a caregiver**, I want to download useful resources, so that I can keep them for later use.

#### Expected Outcome

The caregiver can download selected materials or resources.

#### Notes

This goal should be explored carefully in later requirements because downloads may involve file formats, storage, and content management decisions.

---

### UG-07 — Share useful content

**As a caregiver**, I want to share useful content with others, so that more people can access relevant guidance.

#### Expected Outcome

The caregiver can share a piece of content through available sharing options.

#### Notes

Sharing supports the social value of the product.

---

### UG-08 — Manage a basic profile

**As a caregiver**, I want to manage a basic profile, so that the product can support a more personalized experience.

#### Expected Outcome

The caregiver can access and manage basic profile information.

#### Notes

This goal is lower priority during Inception because authentication and profile management are not part of the current implementation scope.

---

### UG-09 — Discover daily tips

**As a caregiver**, I want to discover short daily tips, so that I can receive practical guidance in a simple format.

#### Expected Outcome

The caregiver can browse or receive short tips related to parenting, rights, or child care.

#### Notes

This goal may become one of the first useful product experiences.

---

### UG-10 — Revisit previously saved content

**As a caregiver**, I want to return to saved content, so that I can review information that I previously considered useful.

#### Expected Outcome

The caregiver can access a list or section of saved content.

#### Notes

This goal depends on the ability to save or bookmark content.

## Candidate Actors for Future Use Cases

The following candidate actors may appear in the initial use case model:

| Actor                 | Description                                                       |
| --------------------- | ----------------------------------------------------------------- |
| Caregiver             | Main user who accesses and interacts with KUNNA content.          |
| Content Administrator | Possible future role responsible for managing content.            |
| Guest User            | Possible user who accesses public content without authentication. |
| Registered User       | Possible user who has a profile and saved preferences.            |

For the first use case model, the main focus should remain on the **Caregiver**.

## Goals Not Prioritized Yet

The following possible goals are not prioritized during the current phase:

- Creating an account.
- Recovering a password.
- Managing advanced personalization.
- Receiving push notifications.
- Creating user-generated content.
- Managing professional or institutional accounts.
- Administering a full content management system.

These goals may be considered in future phases, but they are not central to the first Inception analysis.

## Relationship with Future Use Cases

The user goals in this document will help define the initial use case model.

Possible future use cases include:

| User Goal                           | Possible Use Case  |
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

These are not final use cases yet. They are candidates for the next artifact.

## Engineering Value

Defining user goals before use cases helps prevent premature implementation.

This document supports the project by:

- Clarifying user intent.
- Connecting product vision with system behavior.
- Preparing the use case model.
- Reducing the risk of building features without purpose.
- Supporting a product-first development approach.

## Open Questions

The following questions remain open:

- Which user goal should become the first implemented feature?
- Should KUNNA support guest users before registered users?
- Which content type is most important for the first iteration?
- Should audio content be included in the first implementation iteration?
- Should saved content require authentication?
- What parts of the original UX/UI prototype best represent these user goals?

## Summary

The initial user goals for KUNNA focus on helping caregivers access, understand, save, search, listen to, download, and share useful content related to children's rights and positive parenting.

These goals will guide the next artifact:

**02 — Use Case Model**
