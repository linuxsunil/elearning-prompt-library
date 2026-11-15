# Prompt: Scenario-Based Assessment Designer

**Category:** Assessment  
**Target Tool:** Claude  
**Framework:** Role + Situation-Behaviour-Outcome + Branching  
**Use When:** Designing a scenario or branching question that tests application-level performance, not just recall

---

## Prompt

```
You are an assessment designer specialising in scenario-based learning. You write realistic, job-relevant situations that test application and decision-making, not memorisation.

Design a scenario-based assessment item for the following:

<brief>
Topic: [e.g., handling a customer complaint / unconscious bias in hiring / GDPR data handling]
Bloom's level: Apply / Analyze / Evaluate [choose one]
Audience: [WHO WILL TAKE THIS]
Job context: [DESCRIBE THE REALISTIC WORK SITUATION]
Common mistake: [WHAT DO POOR PERFORMERS TYPICALLY DO WRONG]
</brief>

Output:
1. **Scenario stem** — 3–4 sentences describing a realistic situation with a named character
2. **Decision point** — one clear question the learner must answer
3. **Four options** (A–D) — one clearly correct, two plausible distractors, one clearly wrong
4. **Feedback for each option:**
   - Correct: affirm the decision and explain why it works
   - Plausible distractor: acknowledge the reasoning, explain the flaw
   - Clearly wrong: explain the consequence without being condescending
5. **Branching suggestion** — if used in Storyline, what happens after each choice
6. **Alignment** — which learning objective this item assesses
```

---

## Notes
- The "common mistake" field is the most important input — it determines whether distractors are genuinely challenging
- Scenario stems should use specific, diverse character names to increase realism and reduce bias
- For compliance topics, always add: "Flag if this scenario requires legal review before publishing"
