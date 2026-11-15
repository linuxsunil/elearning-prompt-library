# Prompt: Storyboard Shell Generator

**Category:** Content Development  
**Target Tool:** Claude  
**Framework:** Role + Template + Few-Shot  
**Use When:** Starting a new module and need a storyboard scaffold fast

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
  1. [OBJECTIVE 1]
  2. [OBJECTIVE 2]
  3. [OBJECTIVE 3]
Delivery tool: [Articulate Rise / Storyline 360 / Custom HTML]
</module_brief>

For each screen, output a row in this format:

| Screen # | Screen Title | Layout Type | On-Screen Text (max 30 words) | Narration Script | Visual/Media Notes | Interaction Type | Branching? |
|----------|-------------|-------------|-------------------------------|------------------|-------------------|------------------|-----------|

Include:
- Title screen
- Objectives screen  
- One scenario/hook screen
- Content screens (one per objective, minimum)
- Knowledge check per objective
- Summary screen
- Final assessment placeholder

Use plain narration language — no jargon, second person ("You"), active voice.
Mark any screen that needs SME review with [SME-REVIEW].
```

---

## Notes
- Adjust "Layout Type" to match your tool's native layouts (e.g., Rise: Accordion, Tabs, Flashcards)
- The 30-word on-screen text limit enforces the redundancy principle automatically
- After generating, run the Cognitive Load Audit on any screen marked heavy
