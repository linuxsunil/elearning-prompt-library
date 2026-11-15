# Prompt: SME Notes → Structured Lesson Plan

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Transform + Merrill's First Principles  
**Use When:** You have raw SME content (interview notes, PDFs, slide dumps) and need a structured lesson plan

---

## Prompt

```
You are an instructional designer applying Merrill's First Principles of Instruction.

Transform the following SME notes into a structured lesson plan:

<sme_notes>
[PASTE RAW SME CONTENT HERE]
</sme_notes>

Context:
- Audience: [e.g., new sales reps, frontline managers, compliance staff]
- Delivery: [e.g., self-paced eLearning, 30-minute module, Articulate Rise]
- Performance goal: [e.g., learner will be able to handle a customer objection without escalating]

Structure the output using Merrill's five principles:
1. **Problem-centred** — open with a real-world task or scenario
2. **Activation** — connect to what learners already know
3. **Demonstration** — show, don't just tell
4. **Application** — practice with feedback
5. **Integration** — transfer to real job context

For each principle, provide:
- Suggested content / activity
- Estimated screen count or time
- Interaction type (read, reflect, drag-drop, scenario, quiz, etc.)

End with a list of media assets the developer will need.
```

---

## Notes
- Fill in the three context lines before running — they dramatically improve output quality
- If SME notes are messy, run a clean-up pass first: "Rewrite these notes as clear, structured bullet points without changing meaning"
- Works well piped into the Storyboard Shell prompt next
