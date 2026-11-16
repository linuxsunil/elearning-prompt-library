# Prompt: Project Scoping & Timeline Estimator

**Category:** Project Management  
**Target Tool:** Claude  
**Framework:** Role + Chapman's Development Ratios + Structured Output  
**Use When:** Responding to a new course request or building a Statement of Work  
**Theory applied:** ADDIE (#41) primary — Rationale: Chapman's ratios map to ADDIE phases; effort estimation structured by phase ensures no phase is under-resourced and stakeholders understand where time goes. Secondary: SAM (#42) — for agile projects, the estimator flags where iterative approximation cycles should replace linear waterfall phases.

---

## Prompt

```
You are a senior eLearning project manager with expertise in development time estimation using Chapman's ratio model and ATD benchmarks.

Estimate the development timeline and effort for the following project:

<project_request>
Course title: [TITLE]
Target duration: [MINUTES of finished content]
Delivery format: [Self-paced eLearning / ILT / Blended / Microlearning]
Interactivity level:
  Level 1 — mostly text and narration, minimal interaction
  Level 2 — quizzes, some branching, standard interactions
  Level 3 — simulations, complex branching, custom interactions
  [CHOOSE ONE]
Source content available: [None / SME notes / PPT deck / Existing course to revise]
Authoring tool: [Articulate Rise / Storyline 360 / Custom HTML / Other]
Team: [Solo ID / ID + Developer / Full team with PM and QA]
SME availability: [High = responsive within 24hrs / Medium = 1-week review cycles / Low = hard to reach]
</project_request>

Deliver:

**1. Effort estimate by ADDIE phase**

| Phase | Tasks | Hours |
|---|---|---|
| Analysis | Needs analysis, audience research, brief sign-off | |
| Design | Outline, storyboard, prototype | |
| Development | Build, media production, review cycles | |
| Review cycles | SME review, stakeholder review, revisions | |
| QA | Functionality, SCORM/xAPI, accessibility | |
| Implementation | LMS upload, testing, launch | |
| **Total** | | |

Chapman's ratios used: Level 1 = 49:1, Level 2 = 122:1, Level 3 = 217:1 (development hours per hour of finished content)

**2. Calendar timeline**
Suggested milestone dates if project starts [TODAY'S DATE], showing:
- Brief sign-off
- Storyboard draft
- Storyboard approved
- Alpha build
- Beta build
- SME review complete
- QA complete
- Launch

**3. Key assumptions**
List every assumption made to produce this estimate.

**4. Risk register**
Top 3 risks with likelihood (H/M/L), impact (H/M/L), and mitigation.

**5. Scope boundary**
What is explicitly NOT included in this estimate.

**6. One-page SOW summary**
Suitable for stakeholder sign-off — 200 words maximum.
```

---

## Notes
- Always share the assumptions list with your stakeholder — it prevents scope creep conversations later
- Chapman ratios are averages; adjust upward for new tools, complex topics, or under-resourced teams
- For agile/SAM projects, replace "Review cycles" with "Iteration sprints" and plan 2–3 prototype rounds
- The SOW summary can be pasted directly into an email or project brief document
