# Story: STORY-017 — Extend opportunity score with outcome-likelihood signals

**Capability:** Outcome-oriented opportunity scoring
**Feature:** Outcome-Signal Scoring
**Business Goal:** BG-002
**Priority:** Must-have
**Hypothesis:** [./hypothesis.md](./hypothesis.md)

---

## Job Story

**When** I'm looking for conversations to engage with that have the highest potential for business outcomes
**I want to** see opportunity scores that factor in outcome-likelihood signals predicting downstream results like DMs, collaborations, and leads
**So I can** focus my engagement efforts on conversations most likely to generate measurable business value rather than just engagement metrics

---

## Acceptance Criteria

1. Given a set of conversations for scoring, when the system applies outcome-likelihood signals, then the scores correlate with actual user-reported outcomes with a coefficient of at least 0.3

2. Given conversations with high outcome-likelihood scores, when I engage with them, then at least 25% of active users self-report measurable outcomes (DMs, collaborations, leads) within 8 weeks

3. Given the outcome-likelihood scoring algorithm, when I compare opportunities, then I can clearly see which factors contributed to the outcome probability versus traditional engagement metrics

4. Given a conversation with mixed signals (high engagement, low outcome likelihood or vice versa), when the system ranks it, then the explanation for the ranking is transparent and understandable

5. Given the outcome-likelihood scoring feature, when I use it regularly, then my engagement time is focused on conversations that ultimately lead to business outcomes rather than just high-engagement posts
