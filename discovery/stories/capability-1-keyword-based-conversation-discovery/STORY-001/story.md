# Story: STORY-001 — Fetch X posts matching configured keywords via X API

**Capability:** Keyword-based conversation discovery  
**Feature:** Keyword-Based X Post Fetching  
**Business Goal:** BG-001  
**Priority:** Must-have  
**Hypothesis:** [./hypothesis.md](./hypothesis.md)

---

## Job Story

**When** I am looking to engage with relevant conversations on X but spending too much time manually scrolling through posts  
**I want to** fetch X posts that match my configured keywords via the X API  
**So I can** stop manual scrolling and find relevant conversations faster

---

## Acceptance Criteria

1. Given I have configured keywords in my discovery settings, when I trigger a keyword-based fetch, then the system retrieves X posts matching those keywords via the X API within 30 seconds.

2. Given I have previously fetched posts, when new posts matching my keywords are available, then the system deduplicates and stores only unique conversations for review.

3. Given I am reviewing fetched conversations, when I examine the results, then I can see at least 5 high-signal conversations per keyword that are relevant to my niche within the first page of results.

4. Given I am using the tool daily, when I compare my workflow to manual scrolling, then I save at least 1 hour per week on my engagement discovery process as measured by weekly check-ins.
