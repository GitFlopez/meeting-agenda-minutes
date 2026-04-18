# Prompt 1 — Meeting Agenda Builder

## Purpose
Generate a structured, time-blocked agenda with owner assignments and outcome types before the meeting starts. Ensures every attendee knows the purpose, comes prepared, and knows what decisions are expected.

---

## Prompt (copy and paste into Claude)

```
You are a professional meeting facilitator. Generate a complete meeting agenda based on the inputs below.

MEETING INPUTS:
- Meeting type: [DECISION / BRAINSTORM / STATUS UPDATE / RETROSPECTIVE / STANDUP / KICKOFF / CLIENT CALL / OTHER]
- Meeting title: [e.g., "Q2 Product Roadmap Review"]
- Date & time: [e.g., "Tuesday April 22, 2:00 PM PDT"]
- Duration: [e.g., "60 minutes"]
- Attendees: [list names and roles, e.g., "Sarah Chen (PM), Marcus Webb (Engineering Lead), Jennifer Tran (Design)"]
- Meeting goal: [1-2 sentences — what does "good" look like at the end of this meeting?]
- Topics to cover: [bullet list of topics, e.g., "• Review Q1 metrics  • Prioritize Q2 features  • Assign owners for 3 initiatives"]
- Decisions needed: [list any explicit decisions the group must make, or write "none"]
- Pre-reads required: [documents/links attendees should review beforehand, or write "none"]
- Special constraints: [e.g., "Hard stop at 60 min", "3 remote attendees", "Record for absent stakeholder"]

OUTPUT FORMAT — produce ALL of the following sections:

**1. MEETING HEADER**
Title | Type | Date/Time | Duration | Facilitator | Notetaker

**2. MEETING GOAL (1 sentence)**
The single outcome that defines success for this meeting.

**3. PRE-READ CHECKLIST**
What attendees must review before joining (with owner and estimated read time).
If none: state "No pre-reads required — come ready to discuss."

**4. TIME-BLOCKED AGENDA**
Format as a table:
| Time | Topic | Owner | Format | Expected Outcome |
- Format options: Inform (one-way update) | Discuss (open dialogue) | Decide (vote or consensus required)
- Allocate time proportionally. Reserve final 5 min for action item review.

**5. GROUND RULES** (tailor to meeting type)
3-5 rules appropriate for this meeting (e.g., "One speaker at a time", "Parking lot for off-topic items", "Phones silenced")

**6. ORGANIZER CHECKLIST** (pre-meeting tasks)
- Calendar invite sent with agenda attached? [ ]
- Pre-reads distributed 24h in advance? [ ]
- Meeting room booked / video link tested? [ ]
- Notetaker confirmed? [ ]
- Decisions pre-framed for attendees? [ ]

**7. PARKING LOT PLACEHOLDER**
Label: "PARKING LOT — Topics raised but not in scope for today:"
(Leave blank — to be filled during meeting)
```

---

## Tips

- **Meeting types:** Choose "DECISION" when you need a concrete yes/no or option selection. Choose "BRAINSTORM" when the goal is generating options, not choosing one. Choose "RETROSPECTIVE" for post-project/sprint reviews.
- **Time allocation:** Claude will suggest time blocks, but override them if your team moves faster or slower than average.
- **Pre-reads matter:** Distributing the agenda with pre-reads 24 hours out has been shown to reduce meeting time by 30% (Harvard Business Review, 2022).
- **Parking lot:** Add this to every meeting. It's the single highest-impact facilitation tool — keeps meetings on track without dismissing ideas.

---

## Example Input

```
Meeting type: DECISION
Meeting title: API Rate Limiting — Architecture Decision
Date & time: Thursday April 24, 10:00 AM PDT
Duration: 45 minutes
Attendees: Sarah Chen (PM), Marcus Webb (Engineering Lead), Aisha Okafor (Backend Engineer), Tyler Reeves (DevOps)
Meeting goal: Decide which of 3 rate limiting approaches to implement for v2.0 launch (target: May 1)
Topics to cover:
• Review 3 proposed approaches (Redis token bucket, NGINX rate limit, API Gateway throttling)
• Evaluate cost, complexity, and timeline for each
• Vote on approach
• Assign implementation owner
Decisions needed: Which rate limiting approach to implement?
Pre-reads required: "Rate Limiting Options.doc" (Marcus, 5 min read), Cost estimate spreadsheet (Tyler, 3 min)
Special constraints: Hard stop at 45 min. Tyler is remote (Pacific time). Decision must be logged in Confluence by EOD.
```
