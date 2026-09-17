# 05 — Risk List

## Document Purpose

This document maintains the current risk register for KUNNA.

The risk list was initially created during **I1 — Inception Package** and is now reviewed as part of **I2 — Elaboration**.

Its purpose is to identify, prioritize, monitor, and mitigate product, domain, technical, learning, documentation, and process risks that may affect the next engineering decisions.

The risk register is a living artifact. Risks may be reduced, reprioritized, refined, added, or retired as new evidence becomes available.

## Context

KUNNA is a personal software engineering project based on an original UX/UI prototype.

I1 established the initial engineering baseline through the product vision, user goals, use case model, supplementary requirements, glossary, development strategy, backlog, AI collaboration policy, decision journal, and ADR-0001.

The project is now in **I2 — Elaboration**.

The purpose of this phase is not to complete all analysis or design before implementation. I2 will reduce uncertainty around a selected architecturally significant use case through focused analysis, selective modeling, an explicit architecture hypothesis, executable Java behavior, automated tests, and evidence-based risk reassessment.

Because KUNNA also has learning and professional portfolio value, engineering decisions must remain driven by product value, risk reduction, evidence, and technical justification. Portfolio value must not override product or engineering reasoning.

## Risk Evaluation Criteria

Each risk is evaluated using the following criteria:

| Criterion   | Meaning                                                               |
| ----------- | --------------------------------------------------------------------- |
| Risk        | What could go wrong.                                                  |
| Area        | The part of the project primarily affected by the risk.               |
| Impact      | How serious the consequences would be if the risk materializes.       |
| Probability | How likely the risk currently appears.                                |
| Priority    | How strongly the risk should influence work during the current phase. |
| Mitigation  | The current action used to reduce, control, or observe the risk.      |
| Status      | The current treatment state of the risk.                              |
| Rationale   | Why the current priority and status are appropriate for I2.           |

Impact and probability describe the nature of the risk.

Priority reflects the current phase and may change even when impact and probability remain similar.

## Priority Model

| Priority       | Meaning                                                                         |
| -------------- | ------------------------------------------------------------------------------- |
| P1 — Drives I2 | The risk should directly influence Elaboration decisions and sequencing.        |
| P2 — Active    | The risk requires active mitigation but does not independently drive the phase. |
| P3 — Monitor   | The risk remains relevant but does not require immediate action.                |

## Status Model

| Status       | Meaning                                                                     |
| ------------ | --------------------------------------------------------------------------- |
| Active       | The risk currently requires mitigation or explicit consideration.           |
| Reduced      | Previous work has materially reduced the risk, but it remains relevant.     |
| Monitor      | Current controls are sufficient and the risk should be observed for change. |
| Retired      | The risk is no longer relevant under current project conditions.            |
| Materialized | The risk has occurred and requires treatment as an active problem.          |

## Current Risk Register

| ID  | Risk                                                                                                                                                                                                       | Area                  | Impact | Probability | Priority | Mitigation                                                                                                                                                                                                               | Status  | I2 Rationale                                                                                                                                                               |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ------ | ----------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| R01 | The project becomes too broad before a focused and useful product slice is established.                                                                                                                    | Product scope         | High   | Medium      | P1       | Limit I2 to one selected architecturally significant use case and the minimum supporting requirements, models, code, and tests needed to evaluate it.                                                                    | Active  | The backlog contains many candidate capabilities, while no first executable product slice has yet been selected.                                                           |
| R02 | The project becomes overdocumented before producing useful executable evidence.                                                                                                                            | Documentation         | Medium | Medium      | P2       | Create or refine an artifact only when it reduces a current risk, clarifies the selected use case, supports a decision, or provides evidence needed by the executable slice.                                             | Active  | I1 produced a broad documentation baseline. I2 must prevent additional analysis from delaying implementation without reducing meaningful uncertainty.                      |
| R03 | The original UX/UI prototype influences product direction too strongly without sufficient evidence about current user needs.                                                                               | Product validation    | High   | Medium      | P1       | Treat prototype-derived capabilities as hypotheses. Select I2 work using documented goals, current risks, explicit assumptions, and available evidence rather than reproducing screens mechanically.                     | Active  | Several candidate capabilities still originate from the prototype, while the current research placeholders do not provide user-validation evidence.                        |
| R04 | AI assistance is accepted without sufficient understanding, verification, or ownership by the project owner.                                                                                               | Learning process      | High   | Medium      | P2       | Require human review, explanation, verification, and modification when necessary before AI-assisted requirements, models, decisions, code, or tests are accepted.                                                        | Active  | I2 introduces domain modeling, architecture, Java implementation, and automated tests, increasing the consequences of superficially accepted AI output.                    |
| R05 | Implementation begins before the selected use case, relevant requirements, domain concepts, and architecture hypothesis are sufficiently clear to make the experiment meaningful.                          | Engineering process   | High   | Low         | P2       | Establish only the minimum analysis needed for the selected slice, then implement early enough to obtain executable evidence and refine the analysis from what is learned.                                               | Reduced | I1 created the initial product and engineering baseline. The remaining concern is not coding too early in general, but coding without enough slice-specific understanding. |
| R06 | UML or formal modeling is applied mechanically without improving analysis, design, communication, or risk reduction.                                                                                       | UML modeling          | Medium | Medium      | P2       | Create Domain Models, SSDs, contracts, interaction diagrams, or other models only when they answer a concrete engineering question.                                                                                      | Active  | I2 introduces modeling activities where unnecessary diagrams could easily become procedural deliverables rather than useful reasoning tools.                               |
| R07 | The hybrid language strategy becomes inconsistent between English technical artifacts and Spanish product or domain content.                                                                               | Documentation quality | Medium | Low         | P3       | Keep repository and technical terminology mainly in English while preserving Spanish where it improves domain accuracy or future user-facing communication.                                                              | Monitor | The language policy is established and has remained reasonably consistent during I1.                                                                                       |
| R08 | Frameworks, APIs, persistence, authentication, databases, or other technical mechanisms are introduced before a demonstrated product or architectural need exists.                                         | Technical scope       | High   | Medium      | P1       | Keep the first executable slice as technically small as practical. Introduce infrastructure or frameworks only when the selected use case or validation strategy provides a concrete justification.                      | Active  | Several I1 artifacts anticipate Spring Boot or an API. I2 must prevent those expectations from becoming automatic architecture decisions.                                  |
| R09 | KUNNA presents family, caregiver, child-related, legal, psychological, health, safety, or child-protection content without sufficient provenance or validation.                                            | Domain sensitivity    | High   | Medium      | P1       | Treat sensitive content as unverified until supported by appropriate authoritative sources or a defined review process. Avoid presenting AI-generated or unsupported guidance as authoritative user-facing content.      | Active  | The domain has potentially high consequences, while a formal content provenance and review process has not yet been established.                                           |
| R10 | Product intent and requirements lose traceability as the project moves into analysis, architecture, code, tests, and validation evidence.                                                                  | Traceability          | High   | Medium      | P1       | Maintain sufficient links among vision, goals, selected use case, supplementary requirements, risks, system operations, decisions, code, tests, issues, pull requests, and validation results.                           | Active  | I2 is the first phase where traceability must extend beyond documentation into executable engineering evidence.                                                            |
| R11 | The backlog becomes a list of documents, modeling tasks, or technologies instead of a prioritized representation of product value and risk.                                                                | Product management    | Medium | High        | P1       | Prioritize work using product value, risk reduction, uncertainty, dependency, and current evidence. Learning value may influence sequencing, but portfolio value must not override product or engineering justification. | Active  | The current post-I1 backlog includes artifact-oriented and technology-oriented candidates whose priorities are not yet sufficiently justified.                             |
| R12 | The repository appears organized but fails to communicate credible professional engineering value to reviewers or recruiters.                                                                              | Portfolio value       | High   | Low         | P3       | Let professional value emerge from explainable decisions, focused history, traceability, executable behavior, tests, and honest documentation rather than from artifact volume.                                          | Monitor | Repository organization is already strong enough for the current phase. Portfolio presentation should not drive I2 product or architecture decisions.                      |
| R13 | Architecture remains theoretical and is accepted without executable evidence that it supports the selected significant use case.                                                                           | Architecture          | High   | Medium      | P1       | Define an explicit architecture hypothesis and test it through a small Java vertical slice with automated verification before treating it as an architectural baseline.                                                  | Active  | Elaboration must reduce architectural uncertainty through evidence rather than diagrams or written structure alone.                                                        |
| R14 | Personal data, preferences, bookmarks, profiles, history, or other caregiver-related information are introduced before the project defines what data is actually necessary and how it should be protected. | Privacy               | High   | Medium      | P2       | Apply data minimization, avoid real personal data during development, and introduce persistence, identity, or personal-data handling only when a selected use case demonstrates a concrete need.                         | Active  | Several candidate capabilities could eventually imply stored personal information, but those data requirements and boundaries are not yet validated.                       |
| R15 | Quality requirements remain too vague to support architecture decisions, acceptance criteria, or meaningful automated tests.                                                                               | Requirements quality  | Medium | High        | P2       | Refine only the quality requirements that materially affect the selected I2 slice and express them in a form that can be evaluated or observed.                                                                          | Active  | The current supplementary specification contains several preliminary qualitative terms that are not yet sufficiently verifiable for implementation decisions.              |

## I2 Priority Risks

The risks that currently drive **I2 — Elaboration** are:

1. **R01 — Product scope becomes too broad.**
2. **R03 — Prototype-derived assumptions dominate product direction.**
3. **R08 — Technology is introduced before a demonstrated need exists.**
4. **R09 — Sensitive domain content lacks sufficient provenance or validation.**
5. **R10 — Traceability does not reach executable evidence.**
6. **R11 — The backlog becomes an artifact or technology inventory.**
7. **R13 — Architecture remains theoretical instead of being tested through executable evidence.**

These risks should influence the selection of the architecturally significant use case, the amount of analysis performed, the architecture hypothesis, the scope of the Java vertical slice, and the evidence required before moving toward Construction.

P1 does not mean that all seven risks must be completely eliminated during I2.

It means they must be explicitly considered when making Elaboration decisions.

## Risk Mitigation Strategy for I2

KUNNA will manage I2 risks through the following approach:

1. Select one architecturally significant use case rather than attempting to elaborate the complete product.
2. Refine only the requirements and supplementary concerns that affect the selected slice.
3. Use UML and operation contracts selectively when they reduce ambiguity or risk.
4. Keep architecture provisional until executable evidence supports it.
5. Build a small Java vertical slice during Elaboration rather than postponing all implementation until Construction.
6. Use automated tests to verify meaningful behavior and support architectural learning.
7. Avoid introducing frameworks, persistence, authentication, APIs, or other infrastructure without a demonstrated need.
8. Maintain sufficient traceability from product intent through code, tests, and validation evidence.
9. Reassess the risk register after evaluating the executable slice.
10. Allow implementation evidence to refine requirements, models, architecture, backlog priorities, and future decisions.

## Relationship with Larman-Inspired Practices

This risk register supports an iterative, risk-aware, use-case-driven, and object-oriented engineering approach influenced by Craig Larman's analysis and design practices.

KUNNA does not treat analysis, UML, contracts, GRASP, or architecture as mandatory sequential deliverables.

These techniques are used selectively when they help:

- Clarify user-visible system behavior.
- Understand relevant domain concepts.
- Identify system operations.
- Assign software responsibilities.
- Compare design alternatives.
- Reduce technical uncertainty.
- Prepare or interpret executable evidence.

Implementation is also a learning mechanism.

Models and decisions may therefore be refined when code and tests reveal new information.

## Current Decision

KUNNA is now operating within **I2 — Elaboration**.

Work will be risk-driven, use-case-focused, selective in documentation and modeling, and supported by executable evidence.

The project will not attempt to complete the full product analysis before implementation.

Instead, it will establish sufficient understanding around one selected use case, formulate and test an architecture hypothesis through a small Java vertical slice, and reassess risks before deciding whether the project is ready to expand implementation during Construction.

## Historical Note

The original risk list was created during **I1 — Inception Package**.

I1 mitigated several initial uncertainties by establishing the product and engineering baseline, but it did not eliminate the need for continued risk management.

In particular, the former risk of beginning implementation before completing the initial baseline has been reduced. I2 now shifts attention toward focused scope, product assumptions, sensitive-domain concerns, traceability, backlog quality, premature technology choices, and executable architectural validation.

The closed I1 milestone remains historical and is not reopened by these refinements.

## Notes

This register will continue to evolve as KUNNA progresses.

Risk priority and status may change when:

- A use case is selected or rejected.
- New product evidence appears.
- Architecture experiments produce results.
- Implementation reveals new constraints.
- Tests expose incorrect assumptions.
- Sensitive data or external services become relevant.
- Construction or later phases introduce new operational concerns.

New risks should be added only when they represent a distinct uncertainty that is not already adequately covered by an existing risk.
