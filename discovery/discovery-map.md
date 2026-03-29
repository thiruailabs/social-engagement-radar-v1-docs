# Discovery Map: Social Engagement Radar

> Quick-reference tree from Business Goal → Capability → Feature → Story.

**Date:** 2026-03-29

---

## BG-001 — Reduce user effort and time-to-action for engagement discovery and reply drafting

### Capability 1: Keyword-based conversation discovery

- Feature 1.1: Keyword-Based X Post Fetching
  - STORY-001: Fetch X posts matching configured keywords via X API
  - STORY-002: Schedule periodic keyword fetch runs
- Feature 1.2: Conversation Storage and Deduplication
  - STORY-003: Store and deduplicate fetched conversations

### Capability 2: Opportunity scoring/ranking

- Feature 2.1: Conversation Scoring
  - STORY-004: Score conversations on engagement signals
  - STORY-005: Score conversations on keyword relevance
- Feature 2.2: Opportunity Ranking
  - STORY-006: Rank conversations by composite opportunity score

### Capability 3: AI reply draft generation

- Feature 3.1: AI Draft Generation
  - STORY-007: Generate AI reply draft for a selected conversation ⚠️ Deliberate Discovery
  - STORY-008: Regenerate draft with alternative tone or angle ⚠️ Deliberate Discovery
- Feature 3.2: Draft Editing and Staging
  - STORY-009: Edit AI-generated draft before approval
  - STORY-010: Stage edited draft for publish approval

### Capability 4: Single-page dashboard

- Feature 4.1: Opportunity Feed View
  - STORY-011: Display ranked opportunity list with conversation context
- Feature 4.2: Draft Review and Publish Flow
  - STORY-012: Show draft alongside conversation and approve/publish from dashboard

### Capability 5: Keyword configuration UI

- Feature 5.1: Keyword Management
  - STORY-013: Add, edit, and remove keywords from discovery configuration
  - STORY-014: Preview estimated conversation volume for a keyword ⚠️ Deliberate Discovery

### Capability 6: API rate limit management

- Feature 6.1: Rate-Aware Fetch Scheduling
  - STORY-015: Track X API usage and throttle fetch requests within rate limits
  - STORY-016: Alert user when API rate limits are approaching

---

## BG-002 — Improve users' downstream business outcomes from timely, meaningful replies

### Capability 7: Outcome-oriented opportunity scoring

- Feature 7.1: Outcome-Signal Scoring
  - STORY-017: Extend opportunity score with outcome-likelihood signals ⚠️ Deliberate Discovery
  - STORY-018: Surface outcome-likelihood score alongside engagement score ⏸ Real Options

### Capability 8: Reply angle diversity

- Feature 8.1: Multi-Angle Draft Generation
  - STORY-019: Generate multiple reply angles for a single conversation ⚠️ Deliberate Discovery
  - STORY-020: Label and present each reply angle by type ⏸ Real Options

### Capability 9: Conversation freshness/timeliness indicators

- Feature 9.1: Freshness Signals
  - STORY-021: Calculate and display conversation freshness score
  - STORY-022: Deprioritize stale conversations in ranked list

### Capability 10: Author fit / audience relevance scoring

- Feature 10.1: Author Fit Scoring
  - STORY-023: Score conversation authors on relevance to builder's niche ⚠️ Deliberate Discovery
  - STORY-024: Incorporate author fit score into opportunity ranking ⏸ Real Options

### Capability 11: Outcome capture and tracking

- Feature 11.1: Outcome Logging
  - STORY-025: Log an outcome against a published reply
  - STORY-026: Display outcome history per reply

### Capability 12: Reply performance feedback loop

- Feature 12.1: Outcome-Driven Score Refinement
  - STORY-027: Aggregate outcome data to identify high-performing reply patterns ⚠️ Deliberate Discovery
  - STORY-028: Adjust opportunity scoring weights based on outcome data ⏸ Real Options

---

## BG-003 — Protect user trust by ensuring zero unintended publishes and strong auditability

### Capability 13: Explicit approval gate

- Feature 13.1: Mandatory Publish Approval
  - STORY-029: Enforce mandatory approval step before any X API post call

### Capability 14: Publish audit trail

- Feature 14.1: Publish Action Logging
  - STORY-030: Log every publish attempt with timestamp, content, and outcome
  - STORY-031: Display publish audit log to user

### Capability 15: Content preview before publish

- Feature 15.1: Pre-Publish Content Preview
  - STORY-032: Show exact content with character count and formatting before approval

### Capability 16: Emergency publish rollback

- Feature 16.1: Post-Publish Rollback
  - STORY-033: Delete a published reply via X API within a time window
  - STORY-034: Mark rolled-back replies in the audit log

### Capability 17: API compliance monitoring

- Feature 17.1: Policy Compliance Checks
  - STORY-035: Scan outgoing content for X policy violations before publish ⚠️ Deliberate Discovery
  - STORY-036: Alert user when content may violate X policies ⏸ Real Options

### Capability 18: Rate limit adherence

- Feature 18.1: Publish Rate Limiting
  - STORY-037: Enforce publish frequency limits per X API policy
  - STORY-038: Queue and delay publishes that exceed rate limits

---

## Legend

- ⚠️ **Deliberate Discovery** — story has a high-uncertainty assumption that should be validated before broader implementation
- ⏸ **Real Options** — story remains deferred until a trigger condition is met and commitment becomes justified
