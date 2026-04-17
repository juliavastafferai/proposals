# Proposal Intake

Two modes: Standard Intake (questions) and Notes Extraction (parse meeting notes). Use whichever fits how the user arrives.

---

## Mode A: Standard Intake

> **AGENT: Ask the 4-5 essentials conversationally — do NOT dump all questions at once. Use the full list below as YOUR reference for follow-ups.**

### Quick Start (ask first)
```
Quick — before I draft:
1. Who's the client? (name, company, industry)
2. What's the project? (what do they need from you?)
3. What are you charging? (single price, or tiers?)
4. Timeline? (when does it start, how long?)
```

Then infer proposal type, style, and ask follow-ups only if needed.

### Full Question Bank (your reference — don't dump on user)

**The Client**
1. **Client name?** (person you're sending the proposal to)
2. **Company name?** (if applicable)
3. **Industry?** (helps with tone and expectations)
4. **How did they find you?** (referral, website, social — useful for the executive summary)

**The Project (ask by detected type)**

*Service / Sales:*
5. **What do they need?** (the problem they're trying to solve)
6. **What will you do?** (your proposed solution — services, deliverables)
7. **What are the deliverables?** (specific items they'll receive)
8. **Any phases or milestones?** (discovery → design → build → launch, etc.)

*Partnership:*
5. **What's the partnership about?** (co-marketing, joint venture, referral, etc.)
6. **What does each party contribute?** (resources, audience, expertise)
7. **Revenue share or co-investment model?**
8. **Duration and exclusivity?**

*Membership:*
5. **What's the membership offer?** (community, course, coaching, hybrid)
6. **Tier structure?** (single tier or multiple levels)
7. **What do members get access to?**
8. **Monthly or annual billing? Price per tier?**

*Sponsorship:*
5. **What's the event or property?** (conference, podcast, community, etc.)
6. **Audience size and demographics?**
7. **What sponsorship levels are available?**
8. **What does each level include?** (logo, booth, speaking slot, etc.)

*Speaking:*
5. **What's the event?** (name, date, audience)
6. **What format?** (keynote, workshop, panel, full-day)
7. **Topic preferences?**
8. **Speaker fee + travel expectations?**

**Timeline**
9. **When does the project/engagement start?**
10. **How long will it take / last?**
11. **Any hard deadlines?** (event date, launch date, etc.)

**Pricing** (skip if already answered by type-specific questions)
12. **What are you charging?** (single price, or good/better/best options?)
13. **If tiers: what's the baseline, and what upgrades are available?**
14. **Payment terms?** (50% upfront, monthly, on completion, etc.)

**Your Credentials** (skip if USER.md has this)
15. **Brief description of you/your business**
16. **Relevant experience for this project?**
17. **Testimonials?** (paste 1-2, or say "none — use placeholders")

**Proposal Style** (infer from industry if possible)
18. **What tone?** Corporate / Consultant / Creative / Minimal / Bold

---

## Mode B: Notes Extraction

When the user pastes meeting notes, a call transcript, or a voice memo transcript:

> **AGENT:**
> 1. Read the notes carefully
> 2. Extract answers to all intake questions above
> 3. Present the extracted brief to the user for confirmation
> 4. Flag anything that's missing or unclear: "⚠️ Not found in notes: {{item}}"
> 5. Ask the user to fill in the gaps before proceeding

**Extraction format:**
```
📋 Extracted from your notes:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Client:       {{extracted_name}}
Company:      {{extracted_company}}
Project:      {{extracted_summary}}
Deliverables: {{extracted_list}}
Timeline:     {{extracted_timeline}}
Budget:       {{extracted_or_missing}}
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
⚠️  Missing: {{list of gaps}}

Does this look right? Fill in the blanks and I'll draft the proposal.
```

---

## Quick Intake (Repeat Client)

```
⚡ QUICK INTAKE

1. Same client, new project? Or new client?
2. Project summary (1-2 sentences):
3. Pricing (single or tiers):
4. Timeline:
5. Anything different from your usual proposals?
```

---

## Handling Partial Answers

> **AGENT:**
> 1. Work with what you have — a proposal with some gaps is better than no proposal
> 2. Flag EVERY gap: "⚠️ Needs your input: {{item}}"
> 3. Critical gaps (client name, project scope, pricing): push for these
> 4. Non-critical gaps (testimonials, exact start date): use placeholders
> 5. NEVER invent scope items — only include what was discussed
