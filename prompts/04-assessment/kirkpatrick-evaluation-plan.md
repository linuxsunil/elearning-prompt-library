# Prompt: Kirkpatrick Evaluation Plan

**Category:** Assessment  
**Target Tool:** Claude  
**Framework:** Role + Kirkpatrick Four Levels + Structured Output  
**Use When:** Designing a training evaluation strategy before or after a course launches — for stakeholder reporting, ROI justification, or continuous improvement  
**Theory applied:** Kirkpatrick Model (#48) primary — Rationale: The four-level model provides a systematic framework to evaluate whether training changed reactions, learning, behaviour, and business results rather than measuring only satisfaction. Secondary: Phillips ROI Model (#49) — when executive buy-in or budget justification is needed, adding a fifth level (ROI calculation) makes the business case concrete.

---

## Prompt

```
You are a training evaluation specialist applying the Kirkpatrick Four-Level Model and Phillips ROI methodology.

Design an evaluation plan for the following training programme:

<programme>
Course title: [TITLE]
Business goal: [WHAT BUSINESS OUTCOME THIS TRAINING SUPPORTS]
Audience: [WHO TOOK OR WILL TAKE IT]
Delivery format: [eLearning / ILT / Blended]
Duration: [HOURS]
Approximate learner count: [NUMBER]
Stakeholders: [WHO NEEDS THE EVALUATION RESULTS]
</programme>

Design evaluation at all four Kirkpatrick levels:

**Level 1 — Reaction (Did they like it?)**
- Survey method and timing
- 5 specific survey questions (Likert scale)
- Minimum acceptable score threshold

**Level 2 — Learning (Did they learn it?)**
- Assessment method (pre/post, knowledge check, skill demo)
- What "learning occurred" looks like in measurable terms
- Pass mark and what happens if learners don't meet it

**Level 3 — Behaviour (Are they doing it?)**
- Observation or reporting method (manager check-in, system data, 360 feedback)
- Timing (30-day, 60-day, 90-day post-training)
- 3 specific observable behaviours to look for
- Who is responsible for this data collection

**Level 4 — Results (Did the business improve?)**
- Business metric(s) that should shift if training worked
- Baseline measurement (what is the number before training?)
- Target and timeframe (what number by when?)
- Data source (where does this metric live?)

**Level 5 — ROI (optional, for executive reporting)**
- Cost inputs: development hours, delivery cost, learner time cost
- Benefit inputs: performance improvement value
- ROI formula: ((Benefit - Cost) / Cost) × 100

Finish with: a one-page evaluation summary suitable for a stakeholder slide.
```

---

## Notes
- Level 3 (behaviour) is most commonly skipped — it requires manager involvement and is worth defending
- If the stakeholder only wants a satisfaction survey, explain what Levels 3 and 4 measure and why they matter
- For compliance training, Level 3 is often tracked automatically via LMS completion and incident data
- Pair with the Stakeholder Update Email prompt to communicate evaluation results
