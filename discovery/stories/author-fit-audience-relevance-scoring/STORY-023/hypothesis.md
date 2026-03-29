# Hypothesis: STORY-023 — Score conversation authors on relevance to builder's niche

**Capability:** Author fit / audience relevance scoring
**Feature:** Author Fit Scoring
**Business Goal:** BG-002

---

## Hypothesis Statement

**We believe** scoring conversation authors on relevance to the builder's niche using profile analysis and content similarity metrics
**will result in** builders engaging with conversations where the original poster and participants are more likely to respond and engage back meaningfully
**We will know this to be true when** at least 40% of replies from high-author-fit conversations receive a response within 24 hours, compared to 15% for random conversations

---

## Linked Assumptions (from Impact Map)

| Assumption ID | Statement                                                                                   | Risk | Validation Method                          |
| ------------- | ------------------------------------------------------------------------------------------- | ---- | ------------------------------------------ |
| A-005         | Author fit scoring can identify participants who are likely to engage back with the builder | High | Track API usage and data freshness metrics |

---

## Riskiest Assumption

**The single assumption that would invalidate this hypothesis if wrong:**
Author fit scoring can identify participants who are likely to engage back with the builder

**Minimum experiment to validate it before full build:**
Implement a basic author fit scoring algorithm that analyzes profile keywords, recent tweet topics, and follower overlap with the builder. Deploy to 5 beta users and track response rates for 100 high-author-fit conversations vs 100 random conversations over a 1-week period. Measure the response rate differential.

---

## Validation Plan

**Validated in:** Phase 2 - Early Beta Testing
**Metric:** Response rate differential (responses within 24 hours for high-author-fit vs random conversations)
**Pass threshold:** High-author-fit conversations show at least 2x higher response rate than random conversations
**Fail action:** Pivot to focus on conversation topic relevance only and defer author fit scoring to Phase 4
