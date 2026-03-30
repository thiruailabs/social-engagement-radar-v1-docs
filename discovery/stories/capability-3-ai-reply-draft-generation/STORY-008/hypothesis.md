# Hypothesis: STORY-008 — Regenerate draft with alternative tone or angle

**Capability:** AI reply draft generation
**Feature:** AI Draft Generation
**Business Goal:** BG-001

---

## Hypothesis Statement

**We believe** providing the ability to regenerate AI reply drafts with alternative tones (professional, casual, humorous) or angles (question-based, value-focused, storytelling)
**will result in** builders finding the perfect reply approach faster and increasing their satisfaction with the draft generation feature
**We will know this to be true when** 85% of users who try regeneration report finding a better draft option, and average draft approval time decreases by 30%

---

## Linked Assumptions (from Impact Map)

| Assumption ID | Statement                                                                          | Risk   | Validation Method                      |
| ------------- | ---------------------------------------------------------------------------------- | ------ | -------------------------------------- |
| A-003         | LLM-generated drafts are close enough to user's voice that editing time is minimal | Medium | Collect user feedback on draft quality |

---

## Riskiest Assumption

**The single assumption that would invalidate this hypothesis if wrong:**
LLM-generated drafts are close enough to user's voice that editing time is minimal

**Minimum experiment to validate it before full build:**
Add regeneration buttons for 3 alternative tones to the draft interface. Deploy to the same 8 beta users from STORY-007. Track usage rates (percentage of users who try regeneration) and collect feedback on whether regenerated drafts are better than originals. Measure if regeneration leads to faster approval times.

---

## Validation Plan

**Validated in:** Phase 1 - Core MVP Testing
**Metric:** Regeneration usage rate and draft approval time improvement
**Pass threshold:** At least 60% of users try regeneration AND average approval time decreases by 20% or more
**Fail action:** Pivot to single-draft generation with manual editing focus and defer regeneration to Phase 3
