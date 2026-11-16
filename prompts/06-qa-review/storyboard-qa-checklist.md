# Prompt: Storyboard QA Review

**Category:** QA & Review  
**Target Tool:** Claude  
**Framework:** Role + Multi-Dimension Review + Severity Rating  
**Use When:** Reviewing a completed storyboard before it goes to development  
**Theory applied:** Cognitive Load Theory (#6) primary — Rationale: Most storyboard quality issues trace back to extraneous cognitive load from poor chunking, redundant text, or unclear structure. Secondary: Gagné's Nine Events (#43) — the structural review checks whether all nine events are present and sequenced correctly.

---

## Prompt

```
You are a senior instructional designer performing a quality review of an eLearning storyboard.

Review the following storyboard for quality issues:

<storyboard>
[PASTE STORYBOARD CONTENT — table, bullet points, or screen-by-screen notes]
</storyboard>

Module context:
- Audience: [WHO]
- Learning objectives: [LIST WITH LO CODES]
- Delivery tool: [Rise / Storyline / Other]
- Theory applied: [FROM MODULE DESIGN — e.g., "Situated Learning (#20)"]

Review across these seven dimensions and rate each issue: Critical / Major / Minor

1. Instructional integrity
   - Do activities align to stated LOs?
   - Are higher-order objectives (Apply, Analyze, Evaluate) tested, not just recalled?
   - Is every LO assessed by at least one item?

2. Gagné event coverage
   - Are all nine events present (attention, objectives, recall, content, guidance, practice, feedback, assessment, transfer)?
   - Are Events 3 (recall) and 9 (transfer) explicitly designed?

3. Cognitive load
   - Any screens overloading working memory?
   - Text-heavy screens, missing chunking, narration duplicating on-screen text?
   - Sentences over 20 words in narration?

4. Narration quality
   - Passive voice, jargon, filler words, corporate-speak?
   - Reading level above FK Grade 10 for narration or Grade 8 for on-screen text?

5. Engagement and interaction density
   - At least 2 non-quiz interactions per 10 minutes of content?
   - Practice activities realistic and job-relevant?

6. Accessibility red flags
   - Color-only information encoding?
   - Missing alt text notes for meaningful images?
   - Autoplay media without learner controls?
   - Timed interactions without learner override?

7. Development feasibility
   - Any requests technically unrealistic for the stated tool?
   - Any interaction types not supported by the authoring tool?

Output: a numbered issue list with:
Dimension | Screen # | Severity | Issue description | Suggested fix

End with: "[X] Critical issues must be resolved before development begins."
```

---

## Notes
- Critical = block development; Major = resolve in first dev review; Minor = nice-to-have
- For large storyboards (20+ screens), review in sections of 10 screens for best output quality
- Save the issue list as a comment in your project tracker or QA log for accountability
- After fixes, re-run the Cognitive Load Audit on any screen flagged as text-heavy
