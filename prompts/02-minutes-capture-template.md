# Prompt 2 — Live Meeting Minutes Capture Template

## Purpose
Generate a fill-in-as-you-go minutes template customized to your meeting's agenda. Captures decisions, action items, parking lot items, risks, and dependencies in real time. Works in Google Docs, Notion, Confluence, or plain text.

---

## Prompt (copy and paste into Claude)

```
You are a professional meeting facilitator and notetaker. Generate a structured meeting minutes capture template based on the agenda below.

MEETING INFO:
- Meeting title: [paste from Agenda Builder output or enter manually]
- Date & time: [e.g., "Thursday April 24, 10:00 AM PDT"]
- Facilitator: [name]
- Notetaker: [name]
- Agenda items: [paste the time-blocked agenda from Prompt 1, or list topics manually]

ATTENDEES:
- Present: [list names]
- Absent / Excused: [list names, or "none"]
- Guests: [external attendees, or "none"]

PREFERENCES:
- Note style: [DETAILED (full discussion notes) | SUMMARY (key points only) | ACTION-FOCUSED (decisions + actions only)]
- Output format: [GOOGLE DOCS ready | NOTION ready | PLAIN TEXT | CONFLUENCE WIKI]

OUTPUT FORMAT — produce ALL of the following sections:

**MEETING MINUTES — [Meeting Title]**
Date: | Time: | Duration: | Location/Link: | Facilitator: | Notetaker:

**ATTENDEES**
✓ Present: [list]
✗ Absent: [list]
○ Guests: [list]

**AGENDA ITEM BLOCKS**
(Generate one block per agenda item — structured as:)

---
**[Agenda Item # — Topic Name]** | Owner: [name] | Time: [allocated minutes]

*Discussion Summary:*
[blank lines for notetaker — 3-5 lines depending on note style selected]

*Decision Made:* [ ] Yes — No decision reached
If yes: [blank line for decision text]
Decision owner: _____________ | Effective: _____________

*Action Items from this topic:*
| # | Action | Owner | Due Date | Priority |
|---|--------|-------|----------|----------|
| 1 | | | | |
| 2 | | | | |

*Risks / Blockers raised:*
[blank line]

---
(Repeat for each agenda item)

**PARKING LOT**
| # | Item | Raised by | Assigned to | Target Resolution |
|---|------|-----------|-------------|-------------------|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

**MASTER ACTION ITEM LIST** (consolidated from all topics)
| # | Action | Owner | Due Date | Priority | Status |
|---|--------|-------|----------|----------|--------|
| 1 | | | | High/Med/Low | Open |

**DECISIONS LOG**
| # | Decision | Made by | Date | Rationale |
|---|----------|---------|------|-----------|
| 1 | | | | |

**RISKS & DEPENDENCIES**
| # | Risk/Dependency | Impact | Owner | Mitigation |
|---|----------------|--------|-------|------------|
| 1 | | H/M/L | | |

**NEXT STEPS**
Next meeting: _____________ | Purpose: _____________
Key milestone to watch before next meeting: _____________

**MEETING EFFECTIVENESS** (optional — 30 seconds)
Did we achieve the meeting goal? [ ] Yes [ ] Partially [ ] No
Rating (1-5): ___  One thing to improve next time: _____________

*Minutes prepared by: [notetaker name] | Distributed: [date/time]*
```

---

## Tips

- **Generate before the meeting, fill during.** Run this prompt the night before so you arrive with a ready-to-fill doc, not a blank page.
- **Action item discipline:** Every action item needs three things to exist: an action verb, an owner, and a due date. If any are missing, the action isn't real.
- **Parking lot is not a trash bin.** Review it at the end of every meeting and assign resolution owners. Items that stay in the parking lot for 3+ meetings are either important (escalate) or irrelevant (delete).
- **Decisions log is gold.** When someone asks "why did we do it this way?" in 6 months, this is the answer.
- **Distribute within 24 hours.** Minutes sent same-day have 3x higher action completion rates than minutes sent a week later.

---

## Example Input

```
Meeting title: API Rate Limiting — Architecture Decision
Date & time: Thursday April 24, 10:00 AM PDT
Facilitator: Sarah Chen
Notetaker: Aisha Okafor
Agenda items:
1. Review 3 rate limiting approaches (15 min) — Marcus Webb
2. Cost & timeline evaluation (10 min) — Tyler Reeves
3. Vote on approach (10 min) — All
4. Assign implementation owner (5 min) — Sarah Chen
5. Action review & wrap (5 min) — Sarah Chen

Present: Sarah Chen, Marcus Webb, Aisha Okafor, Tyler Reeves
Absent: None
Guests: None

Note style: SUMMARY
Output format: GOOGLE DOCS ready
```
