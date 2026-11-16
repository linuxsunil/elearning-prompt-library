# Prompt: Storyboard Shell Generator

**Category:** Content Development  
**Target Tool:** Claude  
**Framework:** Role + Template + Gagné Structure  
**Use When:** Starting a new module and need a storyboard scaffold fast  
**Theory applied:** Gagné's Nine Events (#43) primary — Rationale: The storyboard structure maps to Gagné's events to ensure every instructional function (attention, recall, practice, feedback, transfer) is built into the design from the start. Secondary: Information Processing Theory (#8) — screen chunking and sequence follow the sensory → working → long-term memory pipeline.

---

## Prompt

```
You are an eLearning developer who writes lean, production-ready storyboards.

Generate a storyboard shell for the following module:

<module_brief>
Title: [MODULE TITLE]
Audience: [WHO WILL TAKE THIS]
Duration: [TARGET MINUTES]
Objectives:
  LO-01: Learners will be able to [VERB] [CONTENT] [CONDITION]
  LO-02: Learners will be able to [VERB] [CONTENT] [CONDITION]
  LO-03: Learners will be able to [VERB] [CONTENT] [CONDITION]
Delivery tool: [Articulate Rise / Storyline 360 / Custom HTML]
Theory applied: [FROM THEORY SELECTOR OUTPUT]
</module_brief>

For each screen, output a row in this format:

| Screen # | Gagné Event | Screen Title | Layout Type | On-Screen Text (max 30 words) | Narration Script | Visual/Media Notes | Interaction Type | LO Mapped | Branching? |
|----------|------------|-------------|-------------|-------------------------------|------------------|-------------------|------------------|-----------|-----------|

Include screens for:
- Title screen (Event 1 — Gain attention)
- Objectives screen (Event 2 — Inform of objectives)
- Recall activation (Event 3 — Stimulate recall)
- Content screens — one per objective minimum (Event 4 — Present content)
- Worked example or guided demo (Event 5 — Provide guidance)
- Practice activity per objective (Event 6 — Elicit performance)
- Feedback screens (Event 7 — Provide feedback)
- Knowledge check per objective (Event 8 — Assess performance)
- Summary and job aid reference (Event 9 — Enhance retention)

Narration rules:
- Second person ("You", "Your team")
- Active voice only
- Maximum 20 words per sentence
- No corporate filler (leverage, synergize, circle back)
- Contractions are fine (you'll, it's)

Mark screens needing SME review with [SME-REVIEW].
Mark screens needing accessibility notes with [A11Y-CHECK].
```

---

## Notes
- The 30-word on-screen text limit enforces the redundancy principle automatically
- After generating, run the Cognitive Load Audit on any screen with heavy narration
- Gagné Event column makes it easy to spot missing instructional functions at a glance
- For Rise: map Layout Type to Rise block types (Accordion, Tabs, Scenario, Knowledge Check, etc.)
