# Prompt: Action Mapping (Cathy Moore)

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Action Mapping + Performance Focus  
**Use When:** A stakeholder has requested a course — use this before agreeing to build anything to identify whether training is actually the right solution and what the minimum viable content is  
**Theory applied:** Action Mapping (#50) — Rationale: Action Mapping starts with the business goal and works backward to the minimum content needed, eliminating information dumps that don't change behaviour. Secondary: Operant Conditioning (#2) — behaviour change requires practice with feedback, not just information exposure.

---

## Prompt

```
You are an instructional designer applying Cathy Moore's Action Mapping methodology.

Work through an action map for the following training request:

<request>
Business goal: [WHAT BUSINESS OUTCOME MUST IMPROVE — e.g., "reduce customer escalations by 20%"]
Requested course title: [WHAT THE STAKEHOLDER ASKED FOR]
Audience: [WHO WILL TAKE IT — role, experience level]
Current situation: [WHAT IS HAPPENING NOW THAT IS WRONG OR MISSING]
</request>

Work through these steps:

**Step 1 — Validate the business goal**
Is this a measurable business outcome? If not, rewrite it as one.

**Step 2 — Identify the behaviours**
What must people DO differently on the job to achieve the goal?
List 3–5 specific, observable behaviours (not "understand" or "know").

**Step 3 — Identify the causes**
For each behaviour gap, identify the real cause:
- [ ] They don't know HOW (skill/knowledge gap → training may help)
- [ ] They know but don't DO it (motivation, environment, process gap → training alone won't fix this)
- [ ] They can't do it due to a system/tool/process barrier (→ training won't fix this)

**Step 4 — Design the practice**
For each behaviour that IS a training problem, design one practice activity:
- Realistic scenario or task
- Decision the learner must make
- Consequence of the wrong choice

**Step 5 — Identify the minimum content**
What is the bare minimum information a learner needs to complete the practice?
List it. Flag anything that is "nice to know" but not required for performance.

**Step 6 — Recommendation**
Should this be a course? If not, what should it be instead (job aid, manager coaching, process change)?
```

---

## Notes
- Step 3 is the most valuable — it prevents building training that cannot solve the problem
- If causes are mostly motivation or environment, tell the stakeholder directly: training is not the solution
- The "minimum content" list in Step 5 often cuts course length by 30–50% compared to a traditional approach
- Share the action map output with the stakeholder before writing a single word of content
