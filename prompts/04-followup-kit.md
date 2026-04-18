# Prompt 4 — Follow-Up Email + Slack / Teams Summary Kit

## Purpose
Generate the full post-meeting communication package: professional follow-up email to attendees, condensed Slack/Teams message for async teams, individual action item reminder DMs, and an async thread-starter for Notion/Confluence/Linear. Send everything within 30 minutes of the meeting ending.

---

## Prompt (copy and paste into Claude)

```
You are a professional project manager creating the post-meeting communication package. Generate all four formats below based on the meeting summary provided.

MEETING SUMMARY:
[Paste your executive briefing from Prompt 3, completed minutes, or any meeting notes]

COMMUNICATION PREFERENCES:
- Tone: [FORMAL (executive/client) | PROFESSIONAL (internal team) | CASUAL (startup/small team)]
- Team setup: [IN-OFFICE | HYBRID | FULLY REMOTE | ASYNC-FIRST]
- Slack/Teams workspace name: [e.g., "Acme Corp" or leave blank]
- Include emojis in Slack message: [YES | NO]
- Action item reminder timing: [24 HOURS after meeting | 48 HOURS | WEEKLY CADENCE]
- Async tool: [NOTION | CONFLUENCE | LINEAR | JIRA | NONE]

---

OUTPUT — produce ALL of the following:

## FORMAT 1: FOLLOW-UP EMAIL (to all attendees)

**Subject:** [Meeting title] — Decisions, Actions & Next Steps ([date])

**Body:**

Hi [all/team/first names],

Thanks for [joining / making time / your focus] today. Here's the recap:

**DECISIONS MADE:**
• [Decision 1]
• [Decision 2]
(If none: "No formal decisions were made — meeting was informational.")

**ACTION ITEMS:**
| Owner | Action | Due |
|-------|--------|-----|
| [name] | [action] | [date] |

**KEY RISKS / BLOCKERS TO WATCH:**
• [Risk 1 — only if present]

**PARKING LOT (to be addressed):**
• [Parked item 1 — only if present]

Next meeting: [date | time | purpose]

Let me know if I missed anything or if any action items need to be updated.

[Signature]

---

## FORMAT 2: SLACK / TEAMS MESSAGE (condensed, scannable)

[Format for Slack/Teams — use bold, bullets, and emoji markers if YES selected. Target: readable in 30 seconds.]

Example structure:
📋 *[Meeting Title] — Quick Recap* ([date])

✅ *Decisions:*
• [Decision 1]

📌 *Actions:*
• [Owner] → [action] by [date]
• [Owner] → [action] by [date]

⚠️ *Watch:* [Risk or blocker — one line]

📅 *Next up:* [Next meeting date + purpose]

Full notes: [link placeholder]

---

## FORMAT 3: INDIVIDUAL OWNER DM TEMPLATES

(Generate one short DM per action item owner — [ACTION_ITEM_REMINDER_TIMING] after the meeting)

For each owner, generate:

> Hi [name] — quick follow-up on today's [meeting title]:
> 
> Your action: **[action item]**  
> Due: **[due date]**
> 
> Any blockers I should know about? Reply here or flag in [Slack channel / Jira / Linear].

---

## FORMAT 4: ASYNC THREAD-STARTER (for Notion / Confluence / Linear / Jira)

**Thread Title:** [Meeting title] — [Date] — Decisions & Actions

**Body (wiki-formatted):**

# [Meeting Title] — [Date]

**Facilitator:** [name] | **Notetaker:** [name] | **Duration:** [x min]

## TL;DR
[2-sentence summary of what happened and what was decided]

## Decisions
- [Decision 1] — Owner: [name]
- [Decision 2] — Owner: [name]

## Action Items
- [ ] [Action] — @[owner] — due [date]
- [ ] [Action] — @[owner] — due [date]

## Parking Lot
- [ ] [Item] — assigned to @[owner] — resolve by [date]

## Risks
- [Risk] — mitigation owner: @[name]

## Next Meeting
[Date | Time | Purpose | Link]

---
*Notes: Full minutes available on request. Decisions are final unless objections are raised within 48 hours.*
```

---

## Tips

- **30-minute rule.** Send the follow-up within 30 minutes of the meeting ending. This is when context is freshest and people are most likely to act. After 24 hours, completion rates drop by 40%.
- **Email vs Slack.** Use email for external/client meetings (creates a paper trail). Use Slack for internal team meetings (lower friction, higher read rate). Do both for important cross-functional meetings.
- **Individual DMs work.** Studies show action completion rates increase 60% when owners receive a direct reminder vs a group email. The DM template makes this low-effort.
- **Async thread-starter.** For async-first teams (especially those using Notion or Confluence as their "source of truth"), this replaces the need for attendees to look up notes — the thread IS the record.
- **"Objections within 48 hours" clause.** Adding this line to your Confluence/Notion post creates a lightweight decision-acceptance mechanism. If no one objects in 48 hours, the decision is considered ratified.

---

## Example Input

```
Meeting summary:
API Rate Limiting Architecture Decision — April 24, 2026
Decisions: Redis token bucket chosen (lowest latency, $120/month infra cost)
Actions: Aisha Okafor → implement Redis rate limiting → due April 30. Sarah Chen → document decision in Confluence → due EOD today.
Risks: Redis cluster failover not tested in prod — Tyler Reeves to test by April 28.
Next meeting: Architecture Review, April 29, 2:00 PM PDT.

Tone: PROFESSIONAL
Team setup: HYBRID
Slack workspace: Acme Engineering
Include emojis: YES
Action item reminder timing: 48 HOURS
Async tool: CONFLUENCE
```
