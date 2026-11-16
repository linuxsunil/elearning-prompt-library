# Prompt: Theory Selector

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Decision Logic + Structured Output  
**Use When:** Starting a new module or course and need to select the right instructional theory before designing anything  
**Theory applied:** This prompt IS the theory selection tool — it applies the full 60-theory library to any brief.

---

## Prompt

```
You are a senior instructional designer with expertise across the full spectrum of learning theory.

Analyze the following project brief and recommend the optimal theory combination for this course:

<brief>
Topic: [WHAT THE COURSE COVERS]
Audience: [WHO WILL TAKE IT — role, experience level, prior knowledge]
Performance gap: [KNOWLEDGE / SKILL / ATTITUDE / MOTIVATION — what are they currently missing?]
Performance goal: [WHAT THEY MUST BE ABLE TO DO AFTER THE COURSE]
Delivery format: [Self-paced eLearning / ILT / Blended / Microlearning / On-the-job]
Constraints: [Time, tools, budget, accessibility, language — anything relevant]
</brief>

Using this decision logic:
1. Identify the performance gap type (knowledge, skill, attitude, or motivation)
2. Identify the audience level (novice, intermediate, expert, adult professional)
3. Identify the delivery context (self-paced, instructor-led, social, on-the-job)
4. Select a primary theory most suited to those three factors
5. Select a secondary theory to address engagement or motivation
6. Identify one learning science principle to apply to assessment design

Deliver:
1. Primary theory recommendation with rationale (2–3 sentences)
2. Secondary theory recommendation with rationale (1–2 sentences)
3. Assessment design principle with rationale (1–2 sentences)
4. Three things this theory combination implies for the course structure
5. One theory you considered and rejected — and why

Format the output as:
Theory applied: [Primary Name] — Rationale: [one sentence]
Secondary theory: [Name] — Rationale: [one sentence]
Assessment principle: [Name] — Rationale: [one sentence]
```

---

## Theory Reference (summarized)

The full 60-theory library is documented in [INSTRUCTIONAL-DESIGN-FOUNDATIONS.md](../../INSTRUCTIONAL-DESIGN-FOUNDATIONS.md).

Quick selection shortcuts:

| Goal | Primary | Secondary |
|---|---|---|
| Change workplace behaviour | Operant Conditioning (#2) | Behaviour Modification (#4) |
| Teach complex technical skill | Cognitive Load Theory (#6) | 4C/ID Model (#46) |
| Build soft skills | Social Learning Theory (#3) | Self-Efficacy (#40) |
| Motivate disengaged learners | ARCS Model (#35) | Self-Determination Theory (#27) |
| Adult professional audience | Andragogy (#28) | Merrill's Principles (#45) |
| Scenario-based learning | Situated Learning (#20) | Problem-Based Learning (#23) |
| Long-term retention | Spaced Practice (#52) | Retrieval Practice (#54) |
| Culture / mindset change | Transformative Learning (#29) | Attribution Theory (#39) |
| Measure effectiveness | Kirkpatrick (#48) | Phillips ROI (#49) |
| Inclusive design | UDL (#51) | Andragogy (#28) |

---

## Notes
- Run this prompt before any storyboard or content work — theory selection shapes everything downstream
- Paste the output into your module outline so the design rationale is documented
- If the brief is unclear, Claude will ask clarifying questions before recommending — this is intentional
