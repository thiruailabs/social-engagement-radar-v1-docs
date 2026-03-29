# Product Vision Board: Social Engagement Radar v1

## Vision Statement

A radar for builders to discover high-value X conversations early and join them with meaningful, human-approved replies in seconds.

## Product

An AI-powered web app with a single-page dashboard that runs keyword-based conversation discovery on X, scores opportunities, generates multiple reply angle drafts, and supports explicit user approval before publishing.

Key mechanisms:

- Keyword-based discovery of recent posts on X
- Opportunity scoring that surfaces only the most promising conversations
- AI reply angle generation and draft replies
- Human review and approval before any publish action
- Optional public trending pages that expose top conversations for distribution

## Target Group

AI builders, indie hackers, technical SaaS founders, and anyone looking to improve their engagement on X. This product is valuable for those who want to grow their presence and influence through meaningful, timely engagement, regardless of their niche or topic area.

Primary context and constraints:

- They want to engage early, not after conversations have cooled
- They value correctness and tone, so they prefer editable drafts and explicit approval
- They want to grow their presence and influence on X through meaningful, timely engagement, regardless of their niche or topic area

## Needs

1. Find worthy conversations in their niche quickly, without endless scrolling
2. Rank opportunities by likelihood of being worth replying to
3. Generate thoughtful reply angles and drafts that match builder expectations
4. Review, edit, and approve replies before publishing
5. Maintain a simple daily workflow that is fast to use and repeatable

## Product Differentiators

- Discovery-first: the product optimizes for finding reply-worthy conversations, not generating generic posts
- Personal voice modeling: over time, the system learns the user's writing style and tone to generate drafts that sound authentically like them
- Approval before action: drafts can be prepared, but publishing only happens after explicit user approval
- High signal over volume: the dashboard shows a small ranked set of top opportunities per day
- Builder-focused niche setup: keyword configuration plus author fit constraints to reduce noise
- Moat via feedback loops: over time, store outcomes to improve scoring and opportunity selection

## Business Goals

> Business goals involve increasing revenue, protecting revenue, or reducing costs. Every capability and feature must trace back to at least one business goal.

| #      | Business Goal                                                                     | Type               | Measurable Target                                                                                                                                                                      | Time Bound                              |
| ------ | --------------------------------------------------------------------------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| BG-001 | Reduce user effort and time-to-action for engagement discovery and reply drafting | Cost reduction     | In MVP beta, at least 60% of active users report saving at least 1 hour per week on their engagement workflow in a weekly check-in                                                     | Within 4 weeks after MVP launch         |
| BG-002 | Improve users' downstream business outcomes from timely, meaningful replies       | Revenue increase   | Within 8 weeks after MVP launch, at least 25% of active users self-report at least one measurable outcome attributable to replies (for example: inbound DMs, collaborations, or leads) | Within 8 weeks after MVP launch         |
| BG-003 | Protect user trust by ensuring zero unintended publishes and strong auditability  | Revenue protection | Over the first 8 weeks after MVP launch, 100% of publish attempts require explicit approval and 0 unintended publishes occur from system actions                                       | Over the first 8 weeks after MVP launch |

## Product Roadmap

### Phase 2 — Product Validation

- User accounts
- Saved keywords per user
- Daily digests or alerts
- Approval and publish audit views
- Basic billing if needed

### Phase 3 — Performance Loop

- Conversation tracking
- Reply outcome capture
- Improved ranking from feedback
- Early trend detection

### Phase 4 — Defensibility Layer

- Personal voice training
- Niche intelligence models
- Builder network discovery
- Response timing guidance
- Conversation graph analysis

### Phase 5 — Expansion

- LinkedIn support
- Multi-platform radar
- Publish integrations with approval
- Growth analytics
- Reply ROI prediction

### Viral & Growth Features

- Public trending pages
- Shareable conversation radar screenshots
- Generated-with attribution on copied replies
- You-were-early badges
- Daily AI conversation reports
- Free no-signup reply generator as top-of-funnel
- Reply ROI predictor

### Long-Term Vision

The product evolves from a conversation radar into an AI social operating system for builders.

- BG-001: Reduce user effort and time-to-action for engagement discovery and reply drafting
- BG-002: Improve users' downstream business outcomes from timely, meaningful replies
- BG-003: Protect user trust by ensuring zero unintended publishes and strong auditability

## Why Stack Trace

> For each business goal, record the "popping the why stack" reasoning.
> Ask "why?" until you reach a measurable business outcome.

### BG-001

- Request: Reduce the time builders spend finding reply-worthy conversations and drafting replies
- Why? -> Manual scanning and generic writing tools do not reliably surface the right conversations early enough
- Why? -> When users act late, engagement value drops and they spend more time compensating manually
- Root business goal: Lower the user's effective cost of engagement so daily usage becomes sustainable

### BG-002

- Request: Increase the chance that replies lead to visible downstream outcomes for builders
- Why? -> Timeliness and relevance drive whether a reply is noticed and builds real momentum
- Why? -> When the system surfaces higher-signal opportunities and drafts better follow-ups, users can engage earlier and more meaningfully
- Root business goal: Improve user revenue-linked outcomes through higher quality engagement moments

### BG-003

- Request: Ensure the product does not publish unintended content and that every publish event is auditable
- Why? -> Trust failures in social publishing can cause immediate reputation damage and user churn
- Why? -> Explicit human approval and an audit trail reduce risk of incorrect automation
- Root business goal: Protect revenue by preserving user trust and minimizing operational mishaps

## Key Risks & Assumptions

Top risks to monitor:

- Reliable access to fresh, high-quality conversation data from X (API limits, pricing changes, scraping detection, bans)
- Opportunity ranking may surface noisy or stale posts, reducing perceived value
- LLM reply drafts may occasionally miss the user's intended technical tone or context
- Publishing integration constraints or policy changes could break the publish workflow

Assumptions that must hold:

- The niche focus and keyword-based discovery can consistently find enough high-signal conversations for users to feel value quickly
- Human approval keeps the workflow safe enough for users to adopt daily
- A small, ranked dashboard (top 10-20 opportunities per day) is sufficient to drive repeated engagement

## Success Criteria

Within the first 8 weeks after MVP launch:

- Users check the dashboard daily as their engagement workflow (at least 50% of active users open the dashboard at least 5 days per week)
- Users repeatedly convert drafts into actions (at least 30% of shown top opportunities result in a user copying or approving a reply draft)
- Users report improved timing and engagement quality (at least 60% of active users agree that replies help them engage earlier and more meaningfully)
- No unintended publishes occur and publish outcomes are recorded with an auditable trail
