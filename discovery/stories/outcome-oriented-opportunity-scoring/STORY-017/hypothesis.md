# Hypothesis: STORY-017 — Extend opportunity score with outcome-likelihood signals

**Capability:** Outcome-oriented opportunity scoring
**Feature:** Outcome-Signal Scoring
**Business Goal:** BG-002

---

## Hypothesis Statement

**We believe** extending the opportunity scoring algorithm with outcome-likelihood signals that predict downstream business results (DMs, collaborations, leads)
**will result in** builders engaging with conversations that have a higher probability of generating measurable business outcomes rather than just engagement metrics
**We will know this to be true when** at least 25% of active users self-report at least one measurable outcome attributable to replies within 8 weeks after MVP launch

---

## Linked Assumptions (from Impact Map)

| Assumption ID | Statement                                                                                                              | Risk | Validation Method                               |
| ------------- | ---------------------------------------------------------------------------------------------------------------------- | ---- | ----------------------------------------------- |
| A-002         | The opportunity scoring can identify conversations where replies are likely to generate outcomes (not just engagement) | High | Analyze user feedback on surfaced opportunities |
| A-006         | At least 25% of active users will experience at least one measurable outcome within 8 weeks                            | High | Conduct weekly check-ins with users             |

---

## Riskiest Assumption

**The single assumption that would invalidate this hypothesis if wrong:**
The opportunity scoring can identify conversations where replies are likely to generate outcomes (not just engagement)

**Minimum experiment to validate it before full build:**
Deploy a simplified version of outcome-likelihood scoring to a small group of beta users (5-10 builders) and track which conversations they engage with versus which lead to actual outcomes (DMs, collaborations, leads) over a 2-week period. Compare the correlation between high outcome-likelihood scores and actual outcomes versus random engagement.

---

## Validation Plan

**Validated in:** Phase 2 - Early Beta Testing
**Metric:** Correlation coefficient between outcome-likelihood scores and actual user-reported outcomes
**Pass threshold:** Correlation coefficient ≥ 0.3 and at least 2 users report measurable outcomes within 2 weeks
**Fail action:** Pivot to focus on engagement-based scoring only and defer outcome-likelihood scoring to Phase 4
