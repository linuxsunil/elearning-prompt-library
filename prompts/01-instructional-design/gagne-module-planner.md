# Prompt: Gagné's Nine Events Module Planner

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Gagné's Nine Events + Structured Output  
**Use When:** Planning a new module's instructional sequence — before writing any content  
**Theory applied:** Gagné's Nine Events of Instruction (#43) — Rationale: The nine events provide a research-backed instructional sequence that covers attention, encoding, practice, feedback, and transfer — ensuring no critical instructional function is missing from the design.

---

## Prompt

```
You are an instructional designer applying Gagné's Nine Events of Instruction.

Plan the instructional sequence for the following module:

<module_brief>
Topic: [WHAT THE MODULE COVERS]
Audience: [WHO WILL TAKE IT]
Duration: [TARGET MINUTES]
Learning objectives:
  1. [OBJECTIVE 1 — use a revised Bloom's verb]
  2. [OBJECTIVE 2]
  3. [OBJECTIVE 3]
Delivery: [Articulate Rise / Storyline 360 / ILT / Blended]
</module_brief>

Map the module to all nine of Gagné's events. For each event, provide:

| Event | Purpose | Suggested Activity | Screen/Slide | Interaction Type | Time (mins) |
|---|---|---|---|---|---|
| 1. Gain attention | Hook the learner | | | | |
| 2. Inform of objectives | Set expectations | | | | |
| 3. Stimulate recall | Activate prior knowledge | | | | |
| 4. Present content | Deliver instruction | | | | |
| 5. Provide guidance | Scaffold understanding | | | | |
| 6. Elicit performance | Practice | | | | |
| 7. Provide feedback | Correct and elaborate | | | | |
| 8. Assess performance | Measure achievement | | | | |
| 9. Enhance retention | Transfer to job | | | | |

After the table:
- Identify which events are most critical for this topic and audience
- Flag any event that is commonly skipped in eLearning and explain the risk of skipping it here
- Suggest a job aid or performance support tool for Event 9
```

---

## Notes
- Events 3 (stimulate recall) and 9 (enhance retention) are most commonly skipped in eLearning — always plan them explicitly
- For short microlearning (<5 mins), events can be compressed but should not be omitted entirely
- Event 7 (feedback) must be specific and elaborative — not just "Correct!" or "Try again"
- Pair with the Storyboard Shell prompt to turn this plan into a full storyboard
