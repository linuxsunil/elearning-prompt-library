# Prompt: Question Bank Generator

**Category:** Assessment  
**Target Tool:** Claude  
**Framework:** Role + Bloom's + Format Constraint  
**Use When:** Building a full question bank for a module or certification, covering multiple Bloom's levels  
**Theory applied:** Retrieval Practice / Testing Effect (#54) primary — Rationale: Regular, varied retrieval of information from memory is one of the most evidence-backed methods for long-term retention; a well-designed question bank supports this. Secondary: Interleaving (#53) — mixing question types and topics across the bank improves retention compared to blocked practice on one objective at a time.

---

## Prompt

```
You are a psychometrician and instructional designer building a valid, defensible question bank.

Generate a question bank for the following module:

<module>
Topic: [TOPIC]
Audience: [AUDIENCE]
Learning objectives:
  LO-01: [OBJECTIVE USING REVISED BLOOM'S VERB]
  LO-02: [OBJECTIVE]
  LO-03: [OBJECTIVE]
Number of questions per objective: [e.g., 5]
Question types needed: [MCQ / True-False / Matching / Fill-in-the-blank / Short scenario]
Pass mark: [e.g., 80%]
</module>

For each question, provide:

| QID | LO | Bloom's Level | Type | Question Stem | Options (A/B/C/D) | Correct | Rationale | Difficulty |
|-----|-----|--------------|------|--------------|-------------------|---------|-----------|-----------|

Quality rules — apply to every item:
- Minimum 4 options for MCQ; one clearly correct answer
- No "all of the above" or "none of the above"
- No negatively phrased stems ("which is NOT...") unless testing critical safety knowledge — flag if used
- Distractors must be plausible — no obviously wrong options
- Each question independently testable (no "based on the previous question...")
- Rationale is one sentence explaining why the correct answer is correct — use this as feedback text
- Difficulty: Easy (Remember/Understand), Medium (Apply/Analyze), Hard (Evaluate/Create)
- Interleave question types — do not group all MCQs together

After the bank:
- Coverage summary: table showing how many items per LO and per Bloom's level
- Flag any objective with fewer than 3 items as under-assessed
```

---

## Notes
- The rationale column doubles as feedback text — paste directly into Storyline or Rise quiz settings
- For formal certifications, add: "Flag any question where the correct answer could be disputed by a SME"
- Export the table to Excel for LMS import formatting using the xlsx skill
- For spaced retrieval campaigns, add: "Tag each item as Week 1 / Week 2 / Week 4 for a spaced repetition schedule"
