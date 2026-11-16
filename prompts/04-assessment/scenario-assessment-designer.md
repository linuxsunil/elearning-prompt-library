# Prompt: Scenario-Based Assessment Designer

**Category:** Assessment  
**Target Tool:** Claude  
**Framework:** Role + Situation-Behaviour-Outcome + Branching  
**Use When:** Designing a scenario or branching question that tests application-level performance, not just recall  
**Theory applied:** Situated Learning (#20) primary — Rationale: Authentic scenarios place the learner in a realistic job context, making assessment measure actual performance rather than memorization. Secondary: Retrieval Practice (#54) — the act of making a decision under realistic conditions strengthens memory more than re-reading content.

---

## Prompt

```
You are an assessment designer specializing in scenario-based learning. You write realistic, job-relevant situations that test application and decision-making, not memorization.

Design a scenario-based assessment item for the following:

<brief>
Topic: [e.g., handling a customer complaint / unconscious bias in hiring / GDPR data handling]
Bloom's level: Apply / Analyze / Evaluate [choose one]
LO mapped: [LO code from module]
Audience: [WHO WILL TAKE THIS]
Job context: [DESCRIBE THE REALISTIC WORK SITUATION IN DETAIL]
Common mistake: [WHAT DO POOR PERFORMERS TYPICALLY DO WRONG — this drives the distractors]
</brief>

Output:
1. Scenario stem — 3–4 sentences describing a realistic situation with a named character (use a diverse, specific name)
2. Decision point — one clear question the learner must answer
3. Four options (A–D):
   - One clearly correct
   - Two plausible distractors (look reasonable but have a specific flaw)
   - One clearly wrong (but not absurd)
4. Feedback for each option:
   - Correct: affirm the decision and explain why it works (elaborative feedback)
   - Plausible distractor: acknowledge the reasoning, then explain the specific flaw (corrective feedback)
   - Clearly wrong: explain the consequence without being condescending
5. Branching suggestion — if used in Storyline, what happens after each choice
6. Alignment: LO code this item assesses and Bloom's level confirmed

Quality checks:
- No "all of the above" or "none of the above"
- No negatively phrased stems ("which is NOT...")
- Distractors must reflect the common mistake identified in the brief
- Scenario character names must be specific and diverse
```

---

## Notes
- The "common mistake" field is the most important input — it determines whether distractors are genuinely challenging
- For compliance topics, add: "Flag if this scenario requires legal review before publishing"
- For branching: each wrong choice should lead to a consequence screen showing the real-world outcome, not just a "that's wrong" message
- Pair with the Question Bank Generator for a full assessment strategy
