# Prompt: Question Bank Generator

**Category:** Assessment  
**Target Tool:** Claude  
**Framework:** Role + Bloom's + Format Constraint  
**Use When:** Building a full question bank for a module or certification, covering multiple Bloom's levels

---

## Prompt

```
You are a psychometrician and instructional designer building a valid, defensible question bank.

Generate a question bank for the following module:

<module>
Topic: [TOPIC]
Audience: [AUDIENCE]
Learning objectives:
  1. [OBJECTIVE 1]
  2. [OBJECTIVE 2]
  3. [OBJECTIVE 3]
Number of questions per objective: [e.g., 5]
Question types needed: [MCQ / True-False / Matching / Fill-in-the-blank / Short scenario]
</module>

For each question, provide:
- Question ID (OBJ1-Q1, OBJ1-Q2, etc.)
- Bloom's level (Remember / Understand / Apply / Analyze)
- Question stem
- Options (for MCQ: 1 correct + 3 distractors; label A–D)
- Correct answer
- Rationale (one sentence explaining why the correct answer is correct)
- Difficulty: Easy / Medium / Hard

Quality rules:
- No "all of the above" or "none of the above"
- No negative phrasing ("which is NOT…") unless testing critical safety knowledge
- Distractors must be plausible — no obviously silly options
- Each question independently testable without reading other questions

Output as a Markdown table, one question per row.
```

---

## Notes
- The rationale field doubles as feedback text — paste directly into Storyline or Rise quiz settings
- For formal certifications, add: "Flag any question where the correct answer could be disputed by a SME"
- Export the table to Excel using the xlsx skill for LMS import formatting
