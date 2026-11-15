# Prompt: Stakeholder Update Email

**Category:** Project Management  
**Target Tool:** Claude  
**Framework:** Role + Status Report Template + Tone Calibration  
**Use When:** Sending a weekly or milestone update to a client, sponsor, or L&D manager

---

## Prompt

```
You are an eLearning project manager writing a clear, professional status update.

Write a stakeholder update email based on this project status:

<status>
Project name: [NAME]
Reporting period: [DATES]
Overall RAG status: [Red / Amber / Green]
Completed this period:
  - [ITEM 1]
  - [ITEM 2]
In progress:
  - [ITEM with % complete]
Blockers / risks:
  - [ANY ISSUES — or "None"]
Next steps (by [DATE]):
  - [ACTION 1]
  - [ACTION 2]
Decisions needed from stakeholder:
  - [DECISION NEEDED — or "None at this time"]
</status>

Email requirements:
- Subject line that includes RAG status and project name
- Opening sentence: one-line summary of where things stand
- Bullet-point body — no paragraph walls
- Tone: [professional and direct / warm and collaborative / urgent]
- Length: under 200 words in the body
- Close with a specific ask or next meeting date, not a generic "let me know"

Do not start with "I hope this email finds you well."
```

---

## Notes
- The RAG status in the subject line helps stakeholders triage their inbox instantly
- Paste your previous email in a follow-up prompt: "Make this consistent in tone with my previous update: [PASTE]"
- For Red status emails, add: "Add a brief recovery plan section after the blockers"
