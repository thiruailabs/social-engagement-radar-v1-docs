# Story: STORY-014 — Preview estimated conversation volume for a keyword

**Capability:** Keyword configuration UI
**Feature:** Keyword Management
**Business Goal:** BG-001
**Priority:** Should-have
**Hypothesis:** [./hypothesis.md](./hypothesis.md)

---

## Job Story

**When** I'm configuring keywords for conversation discovery and want to understand their potential impact
**I want to** see estimated conversation volumes for each keyword before adding them to my configuration
**So I can** make more effective keyword choices with better signal-to-noise ratios and reduce trial-and-error frustration

---

## Acceptance Criteria

1. Given a keyword I'm considering for configuration, when I view the volume preview, then I see an estimated conversation count for the past 24-48 hours with clear indication of the time period

2. Given multiple keywords in my configuration process, when I compare volume estimates, then I can easily identify which keywords are likely to surface more or fewer conversations

3. Given a volume estimate for a keyword, when I add it to my configuration, then the actual conversation discovery aligns closely with the preview estimate (within 20% variance)

4. Given the volume preview feature, when I configure my keywords, then at least 75% of my selections are for keywords that ultimately surface high-signal conversations

5. Given the volume preview during configuration, when I complete the setup process, then I report at least 70% satisfaction with the keyword configuration experience
