# Features & Stories: Social Engagement Radar

**Date:** 2026-03-29
**Source:** impact-map.md

> U Score = Uncertainty Score: 1 (well understood) → 5 (highly uncertain or novel)
> Deliberate Discovery = stories tackled early to reduce the most important uncertainty  
> Real Options = stories deferred until another story or validation outcome resolves a trigger condition

---

## Capability 1: Keyword-based conversation discovery

**Impact Map Reference:** BG-001 (via Builder)

### Feature 1.1: Keyword-Based X Post Fetching

**Description:** Fetch conversations from X API based on configured keywords to discover relevant engagement opportunities.

| Story ID  | Story Title                                          | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ---------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-001 | Fetch X posts matching configured keywords via X API | 3       | No                   | No           | —          |
| STORY-002 | Schedule periodic keyword fetch runs                 | 2       | No                   | No           | —          |

### Feature 1.2: Conversation Storage and Deduplication

**Description:** Store fetched conversations locally and remove duplicates to ensure users see unique opportunities.

| Story ID  | Story Title                                 | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-003 | Store and deduplicate fetched conversations | 2       | No                   | No           | —          |

---

## Capability 2: Opportunity scoring/ranking

**Impact Map Reference:** BG-001 (via Builder)

### Feature 2.1: Conversation Scoring

**Description:** Evaluate conversations on multiple signals to determine their engagement potential and relevance.

| Story ID  | Story Title                               | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ----------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-004 | Score conversations on engagement signals | 3       | No                   | No           | —          |
| STORY-005 | Score conversations on keyword relevance  | 3       | No                   | No           | —          |

### Feature 2.2: Opportunity Ranking

**Description:** Combine multiple scoring signals to rank conversations and present the most promising opportunities first.

| Story ID  | Story Title                                       | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-006 | Rank conversations by composite opportunity score | 2       | No                   | No           | —          |

---

## Capability 3: AI reply draft generation

**Impact Map Reference:** BG-001 (via Builder)

### Feature 3.1: AI Draft Generation

**Description:** Generate AI-powered reply drafts that match the user's voice and add genuine value to conversations.

| Story ID  | Story Title                                         | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | --------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-007 | Generate AI reply draft for a selected conversation | 4       | Yes (A-003)          | No           | —          |
| STORY-008 | Regenerate draft with alternative tone or angle     | 4       | Yes (A-003)          | No           | —          |

### Feature 3.2: Draft Editing and Staging

**Description:** Allow users to refine AI-generated drafts and prepare them for approval and publishing.

| Story ID  | Story Title                             | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | --------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-009 | Edit AI-generated draft before approval | 2       | No                   | No           | —          |
| STORY-010 | Stage edited draft for publish approval | 2       | No                   | No           | —          |

---

## Capability 4: Single-page dashboard

**Impact Map Reference:** BG-001 (via Builder)

### Feature 4.1: Opportunity Feed View

**Description:** Present ranked engagement opportunities in a clean, focused feed that replaces manual X scrolling.

| Story ID  | Story Title                                               | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | --------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-011 | Display ranked opportunity list with conversation context | 2       | No                   | No           | —          |

### Feature 4.2: Draft Review and Publish Flow

**Description:** Enable users to review drafts alongside conversations and approve publishing in a streamlined workflow.

| Story ID  | Story Title                                                          | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | -------------------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-012 | Show draft alongside conversation and approve/publish from dashboard | 3       | No                   | No           | —          |

---

## Capability 5: Keyword configuration UI

**Impact Map Reference:** BG-001 (via Builder)

### Feature 5.1: Keyword Management

**Description:** Provide intuitive interface for users to configure and manage their discovery keywords.

| Story ID  | Story Title                                                 | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ----------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-013 | Add, edit, and remove keywords from discovery configuration | 1       | No                   | No           | —          |
| STORY-014 | Preview estimated conversation volume for a keyword         | 4       | Yes (A-001)          | No           | —          |

---

## Capability 6: API rate limit management

**Impact Map Reference:** BG-001 (via X Platform)

### Feature 6.1: Rate-Aware Fetch Scheduling

**Description:** Manage X API usage to maintain data freshness while respecting platform rate limits.

| Story ID  | Story Title                                                      | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ---------------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-015 | Track X API usage and throttle fetch requests within rate limits | 3       | No                   | No           | —          |
| STORY-016 | Alert user when API rate limits are approaching                  | 2       | No                   | No           | —          |

---

## Capability 7: Outcome-oriented opportunity scoring

**Impact Map Reference:** BG-002 (via Builder)

### Feature 7.1: Outcome-Signal Scoring

**Description:** Enhance opportunity scoring with signals that predict downstream business outcomes like DMs and collaborations.

| Story ID  | Story Title                                                 | U Score | Deliberate Discovery | Real Options | RO Trigger                                                      |
| --------- | ----------------------------------------------------------- | ------- | -------------------- | ------------ | --------------------------------------------------------------- |
| STORY-017 | Extend opportunity score with outcome-likelihood signals    | 5       | Yes (A-002)          | No           | —                                                               |
| STORY-018 | Surface outcome-likelihood score alongside engagement score | 3       | No                   | Yes          | When STORY-017 validates outcome-likelihood scoring feasibility |

---

## Capability 8: Reply angle diversity

**Impact Map Reference:** BG-002 (via Builder)

### Feature 8.1: Multi-Angle Draft Generation

**Description:** Generate diverse reply approaches to increase engagement probability and conversation participation.

| Story ID  | Story Title                                              | U Score | Deliberate Discovery | Real Options | RO Trigger                                              |
| --------- | -------------------------------------------------------- | ------- | -------------------- | ------------ | ------------------------------------------------------- |
| STORY-019 | Generate multiple reply angles for a single conversation | 4       | Yes (A-003)          | No           | —                                                       |
| STORY-020 | Label and present each reply angle by type               | 3       | No                   | Yes          | When STORY-019 validates multi-angle generation quality |

---

## Capability 9: Conversation freshness/timeliness indicators

**Impact Map Reference:** BG-002 (via Builder)

### Feature 9.1: Freshness Signals

**Description:** Help users prioritize timely conversations by showing age and activity freshness indicators.

| Story ID  | Story Title                                        | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | -------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-021 | Calculate and display conversation freshness score | 2       | No                   | No           | —          |
| STORY-022 | Deprioritize stale conversations in ranked list    | 2       | No                   | No           | —          |

---

## Capability 10: Author fit / audience relevance scoring

**Impact Map Reference:** BG-002 (via Builder)

### Feature 10.1: Author Fit Scoring

**Description:** Score conversation authors on relevance to the builder's niche to improve outcome probability.

| Story ID  | Story Title                                                | U Score | Deliberate Discovery | Real Options | RO Trigger                                           |
| --------- | ---------------------------------------------------------- | ------- | -------------------- | ------------ | ---------------------------------------------------- |
| STORY-023 | Score conversation authors on relevance to builder's niche | 5       | Yes (A-005)          | No           | —                                                    |
| STORY-024 | Incorporate author fit score into opportunity ranking      | 3       | No                   | Yes          | When STORY-023 validates author fit scoring accuracy |

---

## Capability 11: Outcome capture and tracking

**Impact Map Reference:** BG-002 (via Builder)

### Feature 11.1: Outcome Logging

**Description:** Enable users to record and track business outcomes from their published replies.

| Story ID  | Story Title                              | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ---------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-025 | Log an outcome against a published reply | 2       | No                   | No           | —          |
| STORY-026 | Display outcome history per reply        | 2       | No                   | No           | —          |

---

## Capability 12: Reply performance feedback loop

**Impact Map Reference:** BG-002 (via Builder)

### Feature 12.1: Outcome-Driven Score Refinement

**Description:** Use outcome data to continuously improve opportunity scoring algorithms and recommendation quality.

| Story ID  | Story Title                                                       | U Score | Deliberate Discovery | Real Options | RO Trigger                                                        |
| --------- | ----------------------------------------------------------------- | ------- | -------------------- | ------------ | ----------------------------------------------------------------- |
| STORY-027 | Aggregate outcome data to identify high-performing reply patterns | 5       | Yes (A-007)          | No           | —                                                                 |
| STORY-028 | Adjust opportunity scoring weights based on outcome data          | 5       | No                   | Yes          | When STORY-027 validates pattern aggregation with sufficient data |

---

## Capability 13: Explicit approval gate

**Impact Map Reference:** BG-003 (via Builder)

### Feature 13.1: Mandatory Publish Approval

**Description:** Require explicit user approval before any content is published to protect reputation and ensure control.

| Story ID  | Story Title                                                | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ---------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-029 | Enforce mandatory approval step before any X API post call | 2       | No                   | No           | —          |

---

## Capability 14: Publish audit trail

**Impact Map Reference:** BG-003 (via Builder)

### Feature 14.1: Publish Action Logging

**Description:** Maintain a complete audit trail of all publish attempts for transparency and incident investigation.

| Story ID  | Story Title                                                    | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | -------------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-030 | Log every publish attempt with timestamp, content, and outcome | 2       | No                   | No           | —          |
| STORY-031 | Display publish audit log to user                              | 2       | No                   | No           | —          |

---

## Capability 15: Content preview before publish

**Impact Map Reference:** BG-003 (via Builder)

### Feature 15.1: Pre-Publish Content Preview

**Description:** Show users exactly what will be published before requiring final approval to prevent surprises.

| Story ID  | Story Title                                                            | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ---------------------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-032 | Show exact content with character count and formatting before approval | 2       | No                   | No           | —          |

---

## Capability 16: Emergency publish rollback

**Impact Map Reference:** BG-003 (via Builder)

### Feature 16.1: Post-Publish Rollback

**Description:** Provide emergency rollback capability to quickly undo unintended publishes and protect user reputation.

| Story ID  | Story Title                                             | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ------------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-033 | Delete a published reply via X API within a time window | 3       | No                   | No           | —          |
| STORY-034 | Mark rolled-back replies in the audit log               | 2       | No                   | No           | —          |

---

## Capability 17: API compliance monitoring

**Impact Map Reference:** BG-003 (via X Platform)

### Feature 17.1: Policy Compliance Checks

**Description:** Monitor outgoing content for potential policy violations to maintain API access and platform compliance.

| Story ID  | Story Title                                                  | U Score | Deliberate Discovery | Real Options | RO Trigger                                        |
| --------- | ------------------------------------------------------------ | ------- | -------------------- | ------------ | ------------------------------------------------- |
| STORY-035 | Scan outgoing content for X policy violations before publish | 4       | Yes (A-005)          | No           | —                                                 |
| STORY-036 | Alert user when content may violate X policies               | 3       | No                   | Yes          | When STORY-035 validates policy scanning approach |

---

## Capability 18: Rate limit adherence

**Impact Map Reference:** BG-003 (via X Platform)

### Feature 18.1: Publish Rate Limiting

**Description:** Enforce publish rate limits to comply with X API policies and maintain reliable integration.

| Story ID  | Story Title                                       | U Score | Deliberate Discovery | Real Options | RO Trigger |
| --------- | ------------------------------------------------- | ------- | -------------------- | ------------ | ---------- |
| STORY-037 | Enforce publish frequency limits per X API policy | 3       | No                   | No           | —          |
| STORY-038 | Queue and delay publishes that exceed rate limits | 3       | No                   | No           | —          |

---

## Deliberate Discovery Order

> Stories marked for Deliberate Discovery are tackled FIRST within their capability.

Priority queue:

1. STORY-017 (U:5) — Outcome-likelihood scoring is novel with no training data; must validate feasibility before committing to the scoring layer
2. STORY-023 (U:5) — Author fit scoring requires author profile analysis with no established approach; validate before building ranking integration
3. STORY-027 (U:5) — Outcome pattern aggregation requires sufficient data volume that may not exist at MVP; validate data sufficiency assumption early
4. STORY-007 (U:4) — Core LLM draft generation assumption (A-003); must validate that drafts are close enough to user voice before building the full draft workflow
5. STORY-008 (U:4) — Regeneration approach depends on STORY-007 outcomes; tackle early to validate the angle-switching mechanism
6. STORY-014 (U:4) — X API search count endpoint availability is uncertain; validate before building keyword volume preview
7. STORY-019 (U:4) — Multi-angle LLM prompt engineering is uncertain; validate diversity and quality before building the angle-labeling layer
8. STORY-035 (U:4) — X policy violation scanning rules are unclear; validate approach (rule-based vs. LLM) before building the alert layer

---

## Real Options Deferred List

| Story ID  | Story Title                                                 | Reason for Deferral                                                                | Trigger to Revisit                           |
| --------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------------- | -------------------------------------------- |
| STORY-018 | Surface outcome-likelihood score alongside engagement score | Outcome-likelihood score UI is premature until scoring algorithm is validated      | When STORY-017 passes quality gates          |
| STORY-020 | Label and present each reply angle by type                  | Angle-type labeling is premature until multi-angle generation quality is confirmed | When STORY-019 passes quality gates          |
| STORY-024 | Incorporate author fit score into opportunity ranking       | Author fit ranking integration is premature until scoring accuracy is confirmed    | When STORY-023 passes quality gates          |
| STORY-028 | Adjust opportunity scoring weights based on outcome data    | Weight adjustment requires sufficient outcome data that won't exist at MVP         | When STORY-027 validates pattern aggregation |
| STORY-036 | Alert user when content may violate X policies              | Policy alert UI is premature until scanning approach is validated                  | When STORY-035 passes quality gates          |

---

## Summary

| Capability                                       | Features | Stories | High Uncertainty | Deliberate Discovery | Real Options |
| ------------------------------------------------ | -------- | ------- | ---------------- | -------------------- | ------------ |
| 1 — Keyword-based conversation discovery         | 2        | 3       | 0                | 0                    | 0            |
| 2 — Opportunity scoring/ranking                  | 2        | 3       | 0                | 0                    | 0            |
| 3 — AI reply draft generation                    | 2        | 4       | 2                | 2                    | 0            |
| 4 — Single-page dashboard                        | 2        | 2       | 0                | 0                    | 0            |
| 5 — Keyword configuration UI                     | 1        | 2       | 1                | 1                    | 0            |
| 6 — API rate limit management                    | 1        | 2       | 0                | 0                    | 0            |
| 7 — Outcome-oriented opportunity scoring         | 1        | 2       | 1                | 1                    | 1            |
| 8 — Reply angle diversity                        | 1        | 2       | 1                | 1                    | 1            |
| 9 — Conversation freshness/timeliness indicators | 1        | 2       | 0                | 0                    | 0            |
| 10 — Author fit / audience relevance scoring     | 1        | 2       | 1                | 1                    | 1            |
| 11 — Outcome capture and tracking                | 1        | 2       | 0                | 0                    | 0            |
| 12 — Reply performance feedback loop             | 1        | 2       | 1                | 1                    | 1            |
| 13 — Explicit approval gate                      | 1        | 1       | 0                | 0                    | 0            |
| 14 — Publish audit trail                         | 1        | 2       | 0                | 0                    | 0            |
| 15 — Content preview before publish              | 1        | 1       | 0                | 0                    | 0            |
| 16 — Emergency publish rollback                  | 1        | 2       | 0                | 0                    | 0            |
| 17 — API compliance monitoring                   | 1        | 2       | 1                | 1                    | 1            |
| 18 — Rate limit adherence                        | 1        | 2       | 0                | 0                    | 0            |
| **Total**                                        | **22**   | **38**  | **8**            | **8**                | **5**        |
