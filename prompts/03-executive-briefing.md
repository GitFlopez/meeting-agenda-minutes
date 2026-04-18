# Prompt 3 — Executive Briefing Doc (1-Pager)

## Purpose
Transform raw meeting notes or completed minutes into a crisp, scannable 1-page executive summary. Formatted for leaders who weren't in the room. Uses BLUF (Bottom Line Up Front) structure — the same format used by the US military, McKinsey, and Amazon.

---

## Prompt (copy and paste into Claude)

```
You are a chief of staff writing an executive briefing memo. Transform the meeting notes below into a crisp, scannable 1-page executive summary for a senior leader who was not in the meeting.

MEETING NOTES:
[Paste your raw notes, completed minutes template, or any combination of notes from the meeting]

CONTEXT:
- Executive audience: [who is reading this — e.g., "CEO", "VP Engineering", "Board of Directors", "Client (non-technical)"]
- Decisions they care most about: [e.g., "budget impact", "timeline", "risk", "headcount"]
- Urgency: [IMMEDIATE (decide today) | THIS WEEK | FYI ONLY]
- Preferred length: [ULTRA-BRIEF (half page) | STANDARD (full page) | DETAILED (1.5 pages)]

OUTPUT FORMAT — produce ALL of the following sections, fitting on 1 page:

---

**EXECUTIVE BRIEFING**
**Re:** [Meeting Title]  
**Date:** [Meeting date]  
**Prepared by:** [Notetaker/Preparer name]  
**For:** [Executive name/role]  
**Classification:** [INTERNAL | CLIENT-FACING | CONFIDENTIAL]

---

**BOTTOM LINE UP FRONT (BLUF)**
[2-3 sentences maximum. What happened, what was decided, what action is needed from the reader. Write this so a busy executive can stop here and still know what matters.]

---

**KEY DECISIONS MADE**
(Bullet list — max 5. Each bullet: decision + rationale + who owns it)
• [Decision 1] — Rationale: [why] — Owner: [name]
• [Decision 2] — Rationale: [why] — Owner: [name]

If no decisions were made: "No decisions required — informational meeting."

---

**ACTION ITEMS** (sorted by priority)
| Priority | Action | Owner | Due Date |
|----------|--------|-------|----------|
| 🔴 High | | | |
| 🟡 Medium | | | |
| 🟢 Low | | | |

---

**RISKS & OPEN ISSUES**
(Max 3 — only items that require executive awareness or intervention)
• [Risk 1]: [Impact if unresolved] — Mitigation owner: [name]
• [Risk 2]: [Impact if unresolved] — Mitigation owner: [name]

If none: "No risks requiring executive attention at this time."

---

**NEXT MILESTONE TO WATCH**
[One sentence: what is the next key date, decision point, or deliverable that the executive should be aware of?]

Next meeting: [date] | Purpose: [one sentence]

---
*Briefing prepared [date] by [name]. Full minutes available on request.*
```

---

## Tips

- **BLUF is not optional.** Write it last (after the rest of the briefing is done), even though it appears first. The best BLUF is the sentence you'd say in an elevator.
- **For client-facing versions:** Remove internal names from risks. Replace "Owner: [name]" with "Owner: [Team/Department]" to avoid exposing org structure to clients.
- **For board-level briefings:** Add a "Financial Impact" line to the BLUF and include budget numbers in Key Decisions. Boards care about money first.
- **For "bad news" meetings:** Lead the BLUF with the problem, then the plan. Don't bury the lede — executives find out anyway and trust goes down when you obscure problems.
- **Ultra-Brief format:** For Slack/Notion CEO updates, use Ultra-Brief. Every word must earn its place.

---

## Example Input

```
Meeting title: API Rate Limiting — Architecture Decision
Date: Thursday April 24, 10:00 AM PDT

Notes:
- Marcus presented 3 options: Redis token bucket, NGINX, API Gateway throttling
- Redis token bucket chosen: lowest latency (8ms vs 45ms), familiar to team, $120/month added infra cost
- Tyler raised risk: Redis cluster failover not yet tested in prod — will affect rate limiting if Redis goes down
- Implementation owner: Aisha Okafor
- Target: rate limiting live by April 30 (1 week before v2.0 launch May 1)
- Sarah will document decision in Confluence by EOD today
- Next meeting: Architecture review April 29 to validate implementation

Executive audience: VP Engineering
Decisions they care most about: timeline, infra cost, launch risk
Urgency: THIS WEEK
Preferred length: STANDARD
```
