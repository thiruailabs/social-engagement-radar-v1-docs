# Impact Map: Social Engagement Radar

## Impact Map: BG-001 — Reduce user effort and time-to-action for engagement discovery and reply drafting

**Date:** 2026-03-28  
**Business Goal:** BG-001  
**Measurable Target:** In MVP beta, at least 60% of active users report saving at least 1 hour per week on their engagement workflow in a weekly check-in.

---

### Why

**Business Goal:** Reduce user effort and time-to-action for engagement discovery and reply drafting.

---

### Who (Actors)

> Whose behavior needs to change for us to achieve this goal?
> Include both actors who help AND actors who might obstruct the goal.

| Actor      | Role in Goal         | Behavior Change Needed                      | Type        |
| ---------- | -------------------- | ------------------------------------------- | ----------- |
| Builder    | Primary beneficiary  | Uses radar daily instead of manual scanning | Beneficiary |
| X Platform | Potential obstructer | Maintains API access and data freshness     | Obstructor  |

#### Builder

- **Context:** AI builders, indie hackers, technical SaaS founders looking to grow their presence on X.
- **Pain Points:** Time-consuming manual scanning for relevant conversations; generic drafting tools that don't surface the right opportunities.
- **Goals:** Engage early in conversations, build authority, generate leads through timely engagement.
- **Technical Comfort:** High — they are builders.
- **Current Process:** Manual searching on X, bookmarking posts, writing replies from scratch.
- **Obstruction Risk:** Could abandon the tool if it surfaces low-quality conversations or drafts don't match their voice; could revert to manual workflow if onboarding friction is too high.

---

### How (Impacts)

#### Builder

**Positive impacts (behaviors that help):**

- Opens radar daily instead of scrolling X manually.
- Reviews ranked opportunities instead of searching.
- Uses AI drafts as starting points instead of writing from scratch.
- Approves and publishes in seconds.

**Negative impacts (behaviors that could hurt):**

- Over-relies on radar and misses conversations outside keyword scope.
- Spends time tweaking keywords instead of engaging.
- Uses drafts without editing, reducing authenticity.

---

### What (Capabilities)

| Capability                           | Triggers Impact                                     | Actor      | Assumption                                                                   |
| ------------------------------------ | --------------------------------------------------- | ---------- | ---------------------------------------------------------------------------- |
| Keyword-based conversation discovery | Builder stops manual scrolling                      | Builder    | Keyword configuration can consistently surface high-signal conversations.    |
| Opportunity scoring/ranking          | Builder reviews only top opportunities              | Builder    | Scoring algorithm surfaces genuinely reply-worthy conversations (not noise). |
| AI reply draft generation            | Builder uses drafts instead of writing from scratch | Builder    | LLM drafts are close enough to user's voice that editing time is minimal.    |
| Single-page dashboard                | Builder has one place for daily workflow            | Builder    | A small ranked set is sufficient to drive repeated engagement.               |
| Keyword configuration UI             | Builder can tune discovery to their niche           | Builder    | Builders can configure keywords that reliably capture their niche.           |
| API rate limit management            | Data stays fresh enough to be actionable            | X Platform | Rate limits can be managed within acceptable data freshness windows.         |

---

### Assumptions Register

| #     | Assumption                                                                                                        | Risk Level | How to Validate                                                |
| ----- | ----------------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------- |
| A-001 | Keyword-based discovery can consistently surface enough high-signal conversations for users to feel value quickly | High       | Measure user engagement and satisfaction in the first 4 weeks. |
| A-002 | Opportunity scoring algorithm surfaces genuinely reply-worthy conversations with low noise                        | High       | Analyze user feedback on surfaced opportunities.               |
| A-003 | LLM-generated drafts are close enough to the user's voice that editing time is minimal                            | Medium     | Collect user feedback on draft quality.                        |
| A-004 | A small ranked set (top 10-20 per day) is sufficient to drive repeated daily engagement                           | Medium     | Monitor daily usage metrics.                                   |
| A-005 | X API rate limits can be managed within acceptable data freshness windows                                         | High       | Track API usage and data freshness metrics.                    |
| A-006 | Builders will adopt a new daily workflow tool if it demonstrably saves time                                       | Medium     | Survey users on time savings after 4 weeks.                    |
| A-007 | The time saved by using the radar (vs. manual scanning) is at least 1 hour per week for 60% of users              | High       | Conduct weekly check-ins with users.                           |

---

### Reverse Impact Map

| Capability                           | → Behavior Change In                                | → Business Goal       | Connected? |
| ------------------------------------ | --------------------------------------------------- | --------------------- | ---------- |
| Keyword-based conversation discovery | Builder stops manual scrolling                      | BG-001 time reduction | ✅         |
| Opportunity scoring/ranking          | Builder reviews only top opportunities              | BG-001 time reduction | ✅         |
| AI reply draft generation            | Builder uses drafts instead of writing from scratch | BG-001 time reduction | ✅         |
| Single-page dashboard                | Builder has one place for daily workflow            | BG-001 time reduction | ✅         |
| Keyword configuration UI             | Builder can tune discovery to their niche           | BG-001 time reduction | ✅         |
| API rate limit management            | Data stays fresh enough to be actionable            | BG-001 time reduction | ✅         |

---

### Prioritization Notes

**High priority (strong impact, low assumption risk):**

- Keyword-based discovery
- Opportunity scoring
- AI draft generation

**Validate first (high assumption risk):**

- Opportunity scoring (A-002)
- AI draft quality (A-003)

**Defer (weak link to goal, or low impact):**

- Personal voice modeling (Phase 4 in roadmap)
- Advanced keyword configuration

---

## Impact Map: BG-002 — Improve users' downstream business outcomes from timely, meaningful replies

**Date:** 2026-03-28  
**Business Goal:** BG-002  
**Measurable Target:** Within 8 weeks after MVP launch, at least 25% of active users self-report at least one measurable outcome attributable to replies (for example: inbound DMs, collaborations, or leads).

---

### Why

**Business Goal:** Improve users' downstream business outcomes from timely, meaningful replies.

---

### Who (Actors)

> Whose behavior needs to change for us to achieve this goal?
> Include both actors who help AND actors who might obstruct the goal.

| Actor      | Role in Goal         | Behavior Change Needed                  | Type        |
| ---------- | -------------------- | --------------------------------------- | ----------- |
| Builder    | Primary beneficiary  | Engages earlier and more meaningfully   | Beneficiary |
| X Platform | Potential obstructer | Maintains API access and data freshness | Obstructor  |

#### Builder

- **Context:** AI builders, indie hackers, technical SaaS founders looking to grow their presence on X.
- **Pain Points:** Time-consuming manual scanning for relevant conversations; generic drafting tools that don't surface the right opportunities.
- **Goals:** Engage early in conversations, build authority, generate leads through timely engagement.
- **Technical Comfort:** High — they are builders.
- **Current Process:** Manual searching on X, bookmarking posts, writing replies from scratch.
- **Obstruction Risk:** Could abandon the tool if it surfaces low-quality conversations or drafts don't match their voice; could revert to manual workflow if onboarding friction is too high.

---

### How (Impacts)

#### Builder

**Positive impacts (behaviors that help):**

- Engages with conversations earlier (before they cool).
- Selects higher-signal opportunities (conversations with active, relevant participants).
- Uses quality drafts that match their voice and add genuine value.
- Tracks which replies led to outcomes (feedback loop).
- Iterates on reply strategy based on outcome data.

**Negative impacts (behaviors that could hurt):**

- Over-relies on AI drafts without adding personal insight, reducing authenticity.
- Engages with too many conversations, diluting quality.
- Focuses on volume over quality of engagement.

---

### What (Capabilities)

| Capability                                   | Triggers Impact                                                          | Actor   | Assumption                                                                                                  |
| -------------------------------------------- | ------------------------------------------------------------------------ | ------- | ----------------------------------------------------------------------------------------------------------- |
| Outcome-oriented opportunity scoring         | Builder stops manual scrolling                                           | Builder | Opportunity scoring can identify conversations where replies are likely to generate outcomes.               |
| Reply angle diversity                        | Builder uses drafts instead of writing from scratch                      | Builder | AI-generated reply angles add enough genuine value that conversation participants are motivated to respond. |
| Conversation freshness/timeliness indicators | Builder engages while conversation is still active                       | Builder | Timeliness of replies is a significant driver of downstream outcomes.                                       |
| Author fit / audience relevance scoring      | Builder identifies conversations with participants likely to engage back | Builder | Author fit scoring can identify participants who are likely to engage back with the builder.                |
| Outcome capture and tracking                 | Builder records DMs, follows, collaborations                             | Builder | Builders will self-report outcomes if the product makes it easy to do so.                                   |
| Reply performance feedback loop              | Outcome data improves future scoring                                     | Builder | Outcome data collected from early users is sufficient to improve scoring within the 8-week window.          |

---

### Assumptions Register

| #     | Assumption                                                                                                             | Risk Level | How to Validate                                                |
| ----- | ---------------------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------- |
| A-001 | Timeliness of replies is a significant driver of downstream outcomes (DMs, collaborations, leads)                      | High       | Measure user engagement and satisfaction in the first 4 weeks. |
| A-002 | The opportunity scoring can identify conversations where replies are likely to generate outcomes (not just engagement) | High       | Analyze user feedback on surfaced opportunities.               |
| A-003 | AI-generated reply angles add enough genuine value that conversation participants are motivated to respond             | Medium     | Collect user feedback on draft quality.                        |
| A-004 | Builders will self-report outcomes if the product makes it easy to do so                                               | Medium     | Survey users on time savings after 4 weeks.                    |
| A-005 | Author fit scoring can identify participants who are likely to engage back with the builder                            | High       | Track API usage and data freshness metrics.                    |
| A-006 | At least 25% of active users will experience at least one measurable outcome within 8 weeks                            | High       | Conduct weekly check-ins with users.                           |
| A-007 | Outcome data collected from early users is sufficient to improve scoring within the 8-week window                      | High       | Monitor daily usage metrics.                                   |

---

### Reverse Impact Map

| Capability                                   | → Behavior Change In                                                     | → Business Goal         | Connected? |
| -------------------------------------------- | ------------------------------------------------------------------------ | ----------------------- | ---------- |
| Outcome-oriented opportunity scoring         | Builder stops manual scrolling                                           | BG-002 revenue increase | ✅         |
| Reply angle diversity                        | Builder uses drafts instead of writing from scratch                      | BG-002 revenue increase | ✅         |
| Conversation freshness/timeliness indicators | Builder engages while conversation is still active                       | BG-002 revenue increase | ✅         |
| Author fit / audience relevance scoring      | Builder identifies conversations with participants likely to engage back | BG-002 revenue increase | ✅         |
| Outcome capture and tracking                 | Builder records DMs, follows, collaborations                             | BG-002 revenue increase | ✅         |
| Reply performance feedback loop              | Outcome data improves future scoring                                     | BG-002 revenue increase | ✅         |

---

### Prioritization Notes

**High priority (strong impact, low assumption risk):**

- Outcome-oriented opportunity scoring
- Reply angle diversity
- Conversation freshness/timeliness indicators

**Validate first (high assumption risk):**

- Author fit scoring (A-005 — hard to validate without data)
- Reply performance feedback loop (A-007 — needs sufficient outcome data)

**Defer (weak link to goal, or low impact):**

- Reply performance feedback loop (Phase 3 in roadmap — needs outcome data first)

---

## Impact Map: BG-003 — Protect user trust by ensuring zero unintended publishes and strong auditability

**Date:** 2026-03-29  
**Business Goal:** BG-003  
**Measurable Target:** Over the first 8 weeks after MVP launch, 100% of publish attempts require explicit approval and 0 unintended publishes occur from system actions.

---

### Why

**Business Goal:** Protect user trust by ensuring zero unintended publishes and strong auditability.

---

### Who (Actors)

> Whose behavior needs to change for us to achieve this goal?
> Include both actors who help AND actors who might obstruct the goal.

| Actor      | Role in Goal         | Behavior Change Needed                     | Type        |
| ---------- | -------------------- | ------------------------------------------ | ----------- |
| Builder    | Primary beneficiary  | Reviews all content before publish         | Beneficiary |
| X Platform | Potential obstructer | Maintains API access and policy compliance | Obstructor  |

#### Builder

- **Context:** AI builders, indie hackers, technical SaaS founders looking to grow their presence on X.
- **Pain Points:** Fear of reputation damage from incorrect automation; need for control over public content.
- **Goals:** Engage safely on X without risking their professional reputation.
- **Technical Comfort:** High — they are builders.
- **Current Process:** Manual review of all content before posting.
- **Obstruction Risk:** Could abandon the tool if they perceive any risk of unintended publishes; could demand overly complex approval workflows that reduce usability.

#### X Platform

- **Context:** Social media platform with strict content policies and automated detection systems.
- **Pain Points:** Need to maintain platform integrity and prevent spam/abuse.
- **Goals:** Prevent policy violations and maintain user trust in the platform.
- **Technical Comfort:** Automated systems with policy enforcement capabilities.
- **Current Process:** Automated content moderation and policy enforcement.
- **Obstruction Risk:** Could ban or restrict API access if the tool is perceived as violating policies or generating spam-like content.

---

### How (Impacts)

#### Builder

**Positive impacts (behaviors that help):**

- Confidently uses the tool knowing all publishes require explicit approval
- Reviews and approves content with peace of mind about safety controls
- Trusts the audit trail to verify all actions were intentional
- Recommends the tool to peers based on reliability and safety

**Negative impacts (behaviors that could hurt):**

- Abandons the tool if they perceive any risk of unintended publishes
- Demands overly complex approval workflows that reduce usability
- Becomes paranoid about reviewing every detail, slowing down workflow
- Stops using the tool entirely if trust is broken by any incident

#### X Platform

**Positive impacts (behaviors that help):**

- Maintains API access for the tool due to compliant usage patterns
- Allows continued integration because of responsible automation practices
- Views the tool as a legitimate publisher rather than a spam risk

**Negative impacts (behaviors that could hurt):**

- Restricts or bans API access if unintended publishes are detected
- Implements stricter rate limits or policy enforcement
- Flags the tool as high-risk for manual review

---

### What (Capabilities)

| Capability                     | Triggers Impact                                 | Actor      | Assumption                                                             |
| ------------------------------ | ----------------------------------------------- | ---------- | ---------------------------------------------------------------------- |
| Explicit approval gate         | Builder must confirm before any publish         | Builder    | Builders will accept a mandatory approval step as necessary for safety |
| Publish audit trail            | All publish attempts are logged with timestamps | Builder    | An audit trail increases user confidence in the system's reliability   |
| Content preview before publish | Builder sees exactly what will be published     | Builder    | Preview functionality reduces anxiety about unintended content         |
| Emergency publish rollback     | Unintended publishes can be quickly undone      | Builder    | Quick rollback capability can recover from rare approval mistakes      |
| API compliance monitoring      | System monitors for policy violations           | X Platform | Compliance monitoring can prevent access restrictions                  |
| Rate limit adherence           | Publish frequency stays within platform limits  | X Platform | Adhering to rate limits maintains API access                           |

---

### Assumptions Register

| #     | Assumption                                                                       | Risk Level | How to Validate                                                |
| ----- | -------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------- |
| A-001 | Builders will accept a mandatory approval step as necessary for safety           | Medium     | Measure user adoption rates and abandonment patterns           |
| A-002 | An audit trail increases user confidence in the system's reliability             | High       | Survey users on trust levels and confidence in safety features |
| A-003 | Preview functionality reduces anxiety about unintended content                   | Medium     | Collect user feedback on the preview feature                   |
| A-004 | Quick rollback capability can recover from rare approval mistakes                | High       | Test rollback functionality and measure recovery time          |
| A-005 | Compliance monitoring can prevent access restrictions                            | High       | Monitor API access and policy violation reports                |
| A-006 | Adhering to rate limits maintains API access                                     | High       | Track API usage metrics and access status                      |
| A-007 | Zero unintended publishes will be achieved and maintained over the first 8 weeks | High       | Monitor publish logs and user incident reports                 |

---

### Reverse Impact Map

| Capability                     | → Behavior Change In                       | → Business Goal         | Connected? |
| ------------------------------ | ------------------------------------------ | ----------------------- | ---------- |
| Explicit approval gate         | Builder reviews all content before publish | BG-003 trust protection | ✅         |
| Publish audit trail            | Builder trusts the system's reliability    | BG-003 trust protection | ✅         |
| Content preview before publish | Builder feels confident about content      | BG-003 trust protection | ✅         |
| Emergency publish rollback     | Builder recovers from mistakes quickly     | BG-003 trust protection | ✅         |
| API compliance monitoring      | X Platform maintains API access            | BG-003 trust protection | ✅         |
| Rate limit adherence           | X Platform allows continued integration    | BG-003 trust protection | ✅         |

---

### Prioritization Notes

**High priority (strong impact, low assumption risk):**

- Explicit approval gate
- Publish audit trail
- Content preview before publish

**Validate first (high assumption risk):**

- Emergency publish rollback (A-004 — critical for trust recovery)
- API compliance monitoring (A-005 — essential for continued operation)

**Defer (weak link to goal, or low impact):**

- Advanced compliance reporting (Phase 4 in roadmap)
- Third-party audit certification (Phase 5 in roadmap)
