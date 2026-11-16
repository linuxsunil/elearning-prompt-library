# Prompt: SME Notes → Structured Lesson Plan

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Transform + Instructional Model  
**Use When:** You have raw SME content (interview notes, PDFs, slide dumps) and need a structured lesson plan  
**Theory applied:** Merrill's First Principles of Instruction (#45) primary — Rationale: Merrill's five principles ensure content is organised around real-world problems with activation, demonstration, application, and integration rather than passive information delivery. Secondary: Andragogy (#28) — adult learners require relevance to job performance and self-direction, shaping how content is framed and sequenced.

---

## Prompt

```
You are an instructional designer applying Merrill's First Principles of Instruction and Knowles' Andragogy.

Transform the following SME notes into a structured lesson plan:

<sme_notes>
[PASTE RAW SME CONTENT HERE]
</sme_notes>

Context:
- Audience: [e.g., new sales reps, frontline managers, compliance staff]
- Delivery: [e.g., self-paced eLearning, 30-minute module, Articulate Rise]
- Performance goal: [e.g., learner will be able to handle a customer objection without escalating]

Structure the output using Merrill's five principles:
1. Problem-centered — open with a real-world task or scenario the learner will face on the job
2. Activation — connect to what learners already know or have experienced
3. Demonstration — show, don't just tell (examples, worked cases, modelled behaviour)
4. Application — practice with realistic feedback, not just a quiz
5. Integration — transfer to real job context (reflection, job aid, action plan)

For each principle, provide:
- Suggested content or activity
- Estimated screen count or time
- Interaction type (read, reflect, drag-drop, scenario, quiz, etc.)
- Bloom's level addressed

End with:
- A list of media assets the developer will need
- Three learning objectives in LO-{module}-{number} format using revised Bloom's verbs
- Theory applied: [Name] — Rationale: [one sentence]
```

---

## Notes
- Fill in the three context lines before running — they dramatically improve output quality
- If SME notes are messy, run a clean-up pass first: "Rewrite these notes as clear, structured bullet points without changing meaning"
- For compliance topics, add: "Flag any claim that requires legal or SME sign-off before publishing"
- Works well piped into the Storyboard Shell prompt next
