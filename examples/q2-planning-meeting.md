# Example: Q2 Planning Meeting — DataSync SaaS (12-person team)

**Scenario:** DataSync is a B2B SaaS company (12 employees) that helps mid-market companies sync data between cloud platforms. Q2 planning meeting with the leadership team. Goal: align on 3 Q2 initiatives and assign DRIs (Directly Responsible Individuals).

---

## PROMPT 1 OUTPUT — Meeting Agenda

**MEETING HEADER**
| Field | Value |
|-------|-------|
| Title | DataSync Q2 Planning — Initiative Prioritization & DRI Assignment |
| Type | DECISION |
| Date/Time | Tuesday April 22, 2026, 2:00 PM PDT |
| Duration | 75 minutes |
| Facilitator | Rachel Kim (COO) |
| Notetaker | Jordan Lee (Chief of Staff) |

---

**MEETING GOAL**
Exit this meeting with 3 Q2 initiatives formally approved, each with a named DRI, resourcing plan, and success metric — documented in Notion before close of business.

---

**PRE-READ CHECKLIST**

| # | Document | Owner | Est. Read Time |
|---|----------|-------|---------------|
| 1 | Q1 Retrospective Deck (slides 1-12) | Rachel Kim | 8 min |
| 2 | Q2 Initiative Proposals (3 options) | Marcus Webb (Engineering) | 10 min |
| 3 | Q2 Revenue Target & Burn Rate | Jennifer Tran (Finance) | 5 min |

*Distribute by Monday April 21, 10:00 AM PDT — 28 hours before meeting.*

---

**TIME-BLOCKED AGENDA**

| Time | Topic | Owner | Format | Expected Outcome |
|------|-------|-------|--------|-----------------|
| 2:00–2:10 | Q1 results snapshot — what worked, what didn't | Rachel Kim | Inform | Shared baseline understanding |
| 2:10–2:30 | Initiative deep-dive: Proposals 1, 2, 3 | Marcus Webb | Inform | All attendees understand each option |
| 2:30–2:50 | Evaluation & scoring | All | Discuss | Score each initiative on 4 criteria |
| 2:50–3:00 | Vote: select 3 Q2 initiatives | All | Decide | 3 initiatives formally selected |
| 3:00–3:10 | DRI assignment + resourcing | Rachel Kim | Decide | Each initiative has a named DRI + team |
| 3:10–3:15 | Action item review + close | Jordan Lee | Decide | All AIs captured, owners confirmed |

---

**GROUND RULES**
1. Pre-reads required — come ready to discuss, not learn for the first time
2. Parking lot for off-topic items — we'll address them after the vote
3. One speaker at a time during scoring discussion
4. Hard stop at 3:15 PM — Rachel has a 3:30 external call
5. Decisions logged to Notion by Jordan within 1 hour of meeting end

---

**ORGANIZER CHECKLIST**
- [x] Calendar invite sent with agenda attached
- [x] Pre-reads distributed 28 hours in advance
- [x] Video link tested (Zoom Room 3)
- [x] Jordan confirmed as notetaker
- [ ] Scoring matrix shared in Notion before meeting

**PARKING LOT**
*(Items raised during meeting but not in scope for today — to be resolved separately)*
1. _(blank — to be filled during meeting)_

---

## PROMPT 2 OUTPUT — Meeting Minutes (filled in)

**MEETING MINUTES — DataSync Q2 Planning — Initiative Prioritization & DRI Assignment**
Date: April 22, 2026 | Time: 2:00–3:12 PM PDT | Facilitator: Rachel Kim | Notetaker: Jordan Lee

**ATTENDEES**
✓ Present: Rachel Kim (COO), Marcus Webb (Engineering Lead), Jennifer Tran (Finance), Aisha Okafor (Product), Tyler Reeves (DevOps), Sam Park (Sales)
✗ Absent: None
○ Guests: None

---

**AGENDA ITEM 1 — Q1 Results Snapshot** | Owner: Rachel Kim | Time: 10 min

*Discussion Summary:*
Q1 ARR hit $842K (+12% QoQ). Churn was 3.2% (target was <3%). Top churn driver: customers couldn't get data syncing set up within 14 days (onboarding friction). NPS dropped from 42 to 38. Enterprise segment (>500 seats) grew 31% — clear signal.

*Decision Made:* ✓ Yes — Q1 learnings inform Q2 initiative scoring (onboarding improvement weighted higher)

*Action Items:*
| # | Action | Owner | Due Date | Priority |
|---|--------|-------|----------|----------|
| 1 | Post Q1 retrospective deck to Notion all-hands channel | Jordan Lee | April 22, EOD | Medium |

---

**AGENDA ITEM 2 — Initiative Deep-Dive: Proposals 1, 2, 3** | Owner: Marcus Webb | Time: 20 min

*Discussion Summary:*
- **Proposal A: Onboarding Flow Redesign** — 6 weeks, 2 engineers + Aisha (PM), estimated impact: reduce time-to-first-sync from 14 days to 5 days, target churn reduction to <2.5%
- **Proposal B: Enterprise API Tier** — 8 weeks, 3 engineers, estimated impact: unlock $250K ARR from 4 pipeline deals currently blocked on API limits
- **Proposal C: Slack Integration** — 4 weeks, 1 engineer + design, estimated impact: +15 NPS points, 20% reduction in support tickets

Sam (Sales) added context: 3 of the 4 Enterprise API pipeline deals have verbal commitments contingent on API tier — this is real revenue.

*Decision Made:* ✓ Yes — All 3 proposals move to scoring (no eliminations before vote)

---

**AGENDA ITEM 3 — Evaluation & Scoring** | Owner: All | Time: 20 min

*Discussion Summary:*
Scored on 4 criteria (1-5 scale each, max 20 points):
1. Revenue impact (direct or churn-prevention)
2. Customer pain severity
3. Engineering complexity (inverse — lower is better)
4. Time to value (how fast can we see results)

| Initiative | Revenue | Pain | Complexity | Time-to-Value | Total |
|-----------|---------|------|-----------|---------------|-------|
| A: Onboarding | 4 | 5 | 3 | 3 | 15 |
| B: Enterprise API | 5 | 4 | 2 | 4 | 15 |
| C: Slack Integration | 2 | 3 | 4 | 5 | 14 |

Tyler raised risk: Enterprise API may require Redis cluster upgrade — adds 1-2 weeks and $800/month infra. Marcus confirmed he'd scoped this.

*Decision Made:* ✓ Yes — All 3 initiatives proceed (scores are close enough that eliminating any would be arbitrary; team has capacity)

---

**AGENDA ITEM 4 — Vote: Select 3 Q2 Initiatives** | Owner: All | Time: 10 min

*Discussion Summary:*
Confirmed unanimous: Proposals A, B, and C all approved for Q2. Prioritized order for resource conflict resolution: B > A > C.

*Decision Made:* ✓ Yes — Q2 initiatives formally selected: (1) Enterprise API Tier, (2) Onboarding Flow Redesign, (3) Slack Integration

---

**AGENDA ITEM 5 — DRI Assignment + Resourcing** | Owner: Rachel Kim | Time: 10 min

*Decision Made:* ✓ Yes — DRI assignments confirmed
- Initiative B (Enterprise API): Marcus Webb (DRI) | Team: Marcus + Tyler + one backend hire (open req)
- Initiative A (Onboarding): Aisha Okafor (DRI) | Team: Aisha + 2 engineers TBD from Marcus's squad
- Initiative C (Slack): Tyler Reeves (DRI) | Team: Tyler + Mei (Design, 20% allocation)

---

**PARKING LOT**
| # | Item | Raised by | Assigned to | Target Resolution |
|---|------|-----------|-------------|-------------------|
| 1 | Backend hire timeline for Enterprise API team | Sam Park | Rachel Kim | By April 25 — affects Enterprise API start date |
| 2 | Redis upgrade cost approval (>$500/month needs CFO sign-off) | Tyler Reeves | Jennifer Tran | By April 24 |

**DECISIONS LOG**
| # | Decision | Made by | Date |
|---|----------|---------|------|
| 1 | Q2 initiatives: Enterprise API Tier, Onboarding Redesign, Slack Integration | All (unanimous) | April 22 |
| 2 | Priority order for resource conflicts: Enterprise API > Onboarding > Slack | Rachel Kim | April 22 |
| 3 | DRI assignments: Marcus (API), Aisha (Onboarding), Tyler (Slack) | Rachel Kim | April 22 |

**MASTER ACTION ITEM LIST**
| # | Action | Owner | Due Date | Priority |
|---|--------|-------|----------|----------|
| 1 | Post Q1 retro deck to Notion | Jordan Lee | April 22 EOD | Medium |
| 2 | Document Q2 decisions in Notion | Jordan Lee | April 22 EOD | High |
| 3 | Confirm backend hire timeline | Rachel Kim | April 25 | High |
| 4 | Submit Redis cost approval to CFO | Jennifer Tran | April 24 | High |
| 5 | Send DRI confirmation emails to each initiative lead | Rachel Kim | April 23 | Medium |
| 6 | Create Q2 initiative tracking board in Notion | Aisha Okafor | April 24 | Medium |

---

## PROMPT 3 OUTPUT — Executive Briefing

**EXECUTIVE BRIEFING**
**Re:** DataSync Q2 Planning — Initiative Prioritization & DRI Assignment
**Date:** April 22, 2026
**Prepared by:** Jordan Lee (Chief of Staff)
**For:** David Park (CEO)
**Classification:** INTERNAL

---

**BOTTOM LINE UP FRONT**
The Q2 planning meeting succeeded: three initiatives selected unanimously, DRIs assigned, resourcing confirmed. Enterprise API Tier is the top priority — it unlocks $250K ARR from 4 pipeline deals with verbal commitments. Two time-sensitive items need your awareness: a backend hire approval and a Redis infrastructure cost sign-off.

---

**KEY DECISIONS MADE**
• **Q2 initiatives approved (unanimous):** Enterprise API Tier (Priority 1), Onboarding Flow Redesign (Priority 2), Slack Integration (Priority 3). All three proceed in Q2.
• **DRI assignments confirmed:** Marcus Webb → Enterprise API | Aisha Okafor → Onboarding | Tyler Reeves → Slack
• **Resource conflict priority:** If engineering capacity conflicts arise, Enterprise API takes resources from other initiatives first.

---

**ACTION ITEMS** (sorted by priority)

| Priority | Action | Owner | Due Date |
|----------|--------|-------|----------|
| 🔴 High | Confirm backend hire timeline (blocks Enterprise API start) | Rachel Kim | April 25 |
| 🔴 High | Submit Redis upgrade cost approval to Jennifer/CFO ($800/mo infra) | Jennifer Tran | April 24 |
| 🔴 High | Document Q2 decisions in Notion (official record) | Jordan Lee | April 22 EOD |
| 🟡 Medium | Send DRI confirmation emails | Rachel Kim | April 23 |
| 🟡 Medium | Create Q2 initiative tracking board in Notion | Aisha Okafor | April 24 |

---

**RISKS & OPEN ISSUES**
• **Backend hire gap:** Enterprise API team needs one backend engineer — the open req. If hiring takes >4 weeks, Marcus's team is understaffed. Rachel is following up April 25 — flag if unresolved by May 1.
• **Redis infra cost:** $800/month added infrastructure cost for Enterprise API needs CFO approval (>$500/month policy). Unblocked by April 24 or Enterprise API start date slips.

---

**NEXT MILESTONE TO WATCH**
Enterprise API Tier kickoff: targeting April 28 pending hire confirmation and Redis approval. If both are green by April 25, we're on track for a May 30 API Tier launch.

Next meeting: Q2 Initiative Kickoffs, April 28, 10:00 AM PDT

---
*Briefing prepared April 22, 2026 by Jordan Lee. Full minutes available in Notion.*

---

## PROMPT 4 OUTPUT — Follow-Up Kit

### FORMAT 1: Follow-Up Email

**Subject:** Q2 Planning — Decisions, Actions & Next Steps (April 22)

Hi team,

Thanks for a productive Q2 planning session. Here's the recap:

**DECISIONS MADE:**
• Q2 initiatives selected (unanimous): Enterprise API Tier (P1), Onboarding Flow Redesign (P2), Slack Integration (P3)
• DRI assignments: Marcus (Enterprise API), Aisha (Onboarding), Tyler (Slack)
• Resource conflict priority order: API > Onboarding > Slack

**ACTION ITEMS:**
| Owner | Action | Due |
|-------|--------|-----|
| Jordan Lee | Post Q1 retro + Q2 decisions to Notion | Today EOD |
| Jennifer Tran | Submit Redis upgrade cost approval | April 24 |
| Rachel Kim | Confirm backend hire timeline | April 25 |
| Rachel Kim | Send DRI confirmation emails | April 23 |
| Aisha Okafor | Create Q2 tracking board in Notion | April 24 |

**RISKS TO WATCH:**
• Backend hire — Rachel following up April 25. Flag to me if unresolved before May 1.
• Redis infra cost approval — $800/month, needs CFO sign-off by April 24.

Next meeting: Q2 Initiative Kickoffs, Monday April 28, 10:00 AM PDT (Zoom Room 3)

Full notes in Notion: [link]

Jordan

---

### FORMAT 2: Slack Message

📋 *Q2 Planning Recap — April 22*

✅ *Decisions (unanimous):*
• Q2 initiatives: Enterprise API (P1) · Onboarding Redesign (P2) · Slack Integration (P3)
• DRIs: Marcus (API) · Aisha (Onboarding) · Tyler (Slack)

📌 *Actions this week:*
• @jordan → Q2 decisions in Notion → EOD today
• @jennifer → Redis cost approval → April 24
• @rachel → Hire timeline + DRI emails → April 23-25
• @aisha → Q2 tracking board → April 24

⚠️ *Watch:* Backend hire + Redis approval must be green by April 25 or Enterprise API start slips.

📅 *Next: Q2 Kickoffs — Monday April 28, 10 AM PDT*

Full notes 👉 [Notion link]

---

### FORMAT 3: Individual Owner DMs (send 48 hours after meeting)

**To: Jennifer Tran**
> Hi Jennifer — 48-hour follow-up from Tuesday's Q2 Planning session:
> 
> Your action: **Submit Redis upgrade cost approval to CFO (est. $800/month additional infra)**
> Due: **April 24**
> 
> Any blockers I should know about? The Enterprise API kickoff is gated on this one. Reply here or ping me in Slack.

**To: Rachel Kim**
> Hi Rachel — 48-hour check-in from Q2 Planning:
> 
> Your actions:
> 1. **Confirm backend hire timeline** — due April 25 (blocks Enterprise API team)
> 2. **Send DRI confirmation emails (Marcus, Aisha, Tyler)** — due April 23
> 
> Both are critical-path for the April 28 kickoffs. Any blockers?

**To: Aisha Okafor**
> Hi Aisha — follow-up from Q2 Planning:
> 
> Your action: **Create Q2 initiative tracking board in Notion**
> Due: **April 24**
> 
> Congrats on the DRI assignment for Onboarding Redesign — big one. Let me know if you need the scoring matrix from Tuesday for the board.

---

### FORMAT 4: Notion Thread-Starter

**Thread Title:** Q2 Planning — April 22, 2026 — Decisions & Actions

---

# Q2 Planning Meeting — April 22, 2026

**Facilitator:** Rachel Kim | **Notetaker:** Jordan Lee | **Duration:** 72 min

## TL;DR
Three Q2 initiatives selected unanimously with DRIs assigned. Enterprise API Tier is Priority 1 — unlocks $250K ARR from pipeline deals. Two items gate the April 28 kickoff: backend hire confirmation and Redis infra cost approval.

## Decisions
- Q2 initiatives: **Enterprise API Tier** (P1), **Onboarding Flow Redesign** (P2), **Slack Integration** (P3) — Owner: All (unanimous)
- DRI: Enterprise API → @marcus | Onboarding → @aisha | Slack → @tyler — Owner: Rachel Kim
- Resource conflict resolution order: API > Onboarding > Slack — Owner: Rachel Kim

## Action Items
- [ ] Post Q1 retro + Q2 decisions to Notion — @jordan — due April 22 EOD
- [ ] Submit Redis cost approval to CFO — @jennifer — due April 24
- [ ] Confirm backend hire timeline — @rachel — due April 25
- [ ] Send DRI confirmation emails — @rachel — due April 23
- [ ] Create Q2 tracking board — @aisha — due April 24

## Parking Lot
- [ ] Backend hire open req timeline — @rachel to resolve by April 25
- [ ] Redis upgrade cost approval (>$500/mo policy) — @jennifer to resolve by April 24

## Risks
- Backend hire gap — blocks Enterprise API team if not resolved by May 1
- Redis infra cost — $800/month, needs CFO approval before April 24

## Next Meeting
April 28, 10:00 AM PDT | Q2 Initiative Kickoffs | Zoom Room 3

---
*Notes: Decisions are final unless objections are raised in this thread within 48 hours (by April 24, 2:00 PM PDT). Full minutes available from @jordan on request.*
