# Example Map: STORY-001 — Fetch X posts matching configured keywords via X API

**Capability:** Keyword-based conversation discovery  
**Feature:** Keyword-Based X Post Fetching  
**Date:** 2026-03-30

---

## Business Rules

| #   | Rule                                                                                       |
| --- | ------------------------------------------------------------------------------------------ |
| R1  | The system must fetch X posts matching configured keywords via the X API when triggered    |
| R2  | The system must complete keyword-based fetch operations within 30 seconds                  |
| R3  | The system must deduplicate previously fetched posts and store only unique conversations   |
| R4  | The system must surface at least 5 high-signal conversations per keyword on the first page |
| R5  | The system must integrate with the X API to retrieve posts based on keyword search queries |
| R6  | The system must handle API rate limiting and error conditions gracefully                   |

---

## Examples

| Rule | Example                                                                                                                                | Path       | Priority |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------- |
| R1   | User triggers keyword fetch with keywords "AI", "machine learning" → system calls X API with search query and retrieves matching posts | Happy path | ⚑        |
| R1   | User triggers fetch with no configured keywords → system shows error message "No keywords configured"                                  | Edge case  | —        |
| R2   | User triggers fetch → system completes retrieval within 25 seconds                                                                     | Happy path | —        |
| R2   | User triggers fetch → system takes 35 seconds and shows timeout error                                                                  | Edge case  | —        |
| R3   | User triggers fetch with keywords that match previously stored posts → system filters out duplicates and stores only new conversations | Happy path | —        |
| R3   | User triggers fetch with all new posts (no duplicates) → system stores all retrieved conversations                                     | Edge case  | —        |
| R4   | User reviews results for keyword "AI" → system displays 7 high-signal conversations on first page                                      | Happy path | ⚑        |
| R4   | User reviews results for keyword "blockchain" → system displays only 2 conversations on first page → system shows "Need more data"     | Edge case  | ⚑        |
| R5   | System makes X API call with valid search parameters → X API returns matching posts                                                    | Happy path | ⚑        |
| R5   | System makes X API call with malformed parameters → X API returns error → system logs and shows user-friendly message                  | Edge case  | ⚑        |
| R6   | X API returns rate limit exceeded error → system implements exponential backoff and retries                                            | Edge case  | ⚑        |
| R6   | X API is temporarily unavailable → system shows connection error and suggests retry                                                    | Edge case  | ⚑        |

> ⚑ = linked to riskiest assumption from hypothesis.md — cover this example first in scenarios

---

## Open Questions

| #   | Question                                                                                           | Owner                      | Target Date |
| --- | -------------------------------------------------------------------------------------------------- | -------------------------- | ----------- |
| Q1  | What specific X API endpoints and authentication methods should be used for post retrieval?        | API Integration Specialist | 2026-04-02  |
| Q2  | How should the system define "high-signal conversations" for deduplication and ranking purposes?   | Product Manager            | 2026-04-03  |
| Q3  | What specific rate limiting strategies should be implemented for the X API integration?            | Infrastructure Specialist  | 2026-04-02  |
| Q4  | How should conversation uniqueness be determined - by post ID, content similarity, or both?        | Lead Developer             | 2026-04-01  |
| Q5  | What constitutes a "high-signal conversation" in terms of engagement metrics and relevance scores? | UX Researcher              | 2026-04-05  |
