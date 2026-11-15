# Prompt: Storyline 360 Trigger & Variable Logic

**Category:** Storyline / Rise Development  
**Target Tool:** Claude / Claude Code  
**Framework:** Role + Specification + Structured Output  
**Use When:** Designing branching logic, variable tracking, or complex trigger sequences in Storyline 360

---

## Prompt

```
You are an Articulate Storyline 360 developer with deep expertise in trigger logic and variable management.

Design the trigger and variable architecture for this interaction:

<interaction_brief>
[DESCRIBE THE INTERACTION — e.g., "A 3-path branching scenario where the learner's choices in slides 3, 7, and 12 determine which of two outcome screens they reach. Correct path requires choosing Option B on slide 3, any option on slide 7, and Option A on slide 12."]
</interaction_brief>

Deliver:
1. **Variable list** — name, type (T/F, number, text), initial value, purpose
2. **Trigger table** — for each trigger: Object | Event | Action | Condition | Target
3. **Slide map** — which slides connect to which, with the condition that controls each branch
4. **Edge cases** — what happens if the learner revisits a slide or uses the Back button
5. **QA checklist** — 5 things to test before publishing

Format the trigger table as Markdown. Use Storyline's exact action names (e.g., "Jump to slide", "Adjust variable", "Show layer").
```

---

## Notes
- Be as specific as possible in the interaction brief — vague briefs produce generic logic
- Paste the output into a comment in your .story file for documentation
- For xAPI/SCORM tracking requirements, add: "This module must report completion only when the learner reaches the success outcome screen"
