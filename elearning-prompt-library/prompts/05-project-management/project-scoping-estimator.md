# Prompt: Project Scoping & Timeline Estimator

**Category:** Project Management  
**Target Tool:** Claude  
**Framework:** Role + Chapman's Development Ratios + Structured Output  
**Use When:** Responding to a new course request or building a Statement of Work

---

## Prompt

```
You are a senior eLearning project manager with expertise in development time estimation using Chapman's ratio model and ATD benchmarks.

Estimate the development timeline and effort for the following project:

<project_request>
Course title: [TITLE]
Target duration: [MINUTES of finished content]
Delivery format: [Self-paced eLearning / ILT / Blended / Microlearning]
Interactivity level: [Level 1 (mostly text/narration) / Level 2 (quizzes, some branching) / Level 3 (simulations, complex branching)]
Source content available: [None / SME notes / PPT deck / Existing course to revise]
Authoring tool: [Articulate Rise / Storyline 360 / Custom HTML / Other]
Team: [Solo ID / ID + Developer / Full team]
SME availability: [High (responsive) / Medium (1-week review cycles) / Low (hard to reach)]
</project_request>

Deliver:
1. **Effort estimate** — hours by phase (Analysis, Design, Development, Review, QA, Launch)
2. **Calendar timeline** — suggested milestone dates if project starts [TODAY'S DATE]
3. **Key assumptions** — what you assumed to produce this estimate
4. **Risk register** — top 3 risks with likelihood (H/M/L) and mitigation
5. **Scope boundary** — what is explicitly NOT included
6. **One-page SOW summary** — suitable for stakeholder sign-off

Use Chapman's ratio for the development phase: Level 1 = 49:1, Level 2 = 122:1, Level 3 = 217:1 (hours of development per hour of finished content).
```

---

## Notes
- Always share the assumptions list with your stakeholder — it prevents scope creep
- Chapman ratios are averages; adjust upward for new tools, complex topics, or under-resourced teams
- The SOW summary section can be pasted directly into an email or project brief
