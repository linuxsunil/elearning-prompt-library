# Prompt: Articulate Rise Block Planner

**Category:** Storyline / Rise Development  
**Target Tool:** Claude  
**Framework:** Role + Constraint + Template  
**Use When:** Planning a Rise 360 course before building — avoids layout mismatches and over-use of Text blocks

---

## Prompt

```
You are an Articulate Rise 360 specialist. Plan the block sequence for the following lesson:

<lesson_brief>
Topic: [TOPIC]
Audience: [AUDIENCE]
Duration target: [MINUTES]
Learning objectives:
  1. [OBJECTIVE 1]
  2. [OBJECTIVE 2]
Key content points: [LIST THE MAIN POINTS OR PASTE SME NOTES]
</lesson_brief>

For each lesson section, recommend a block sequence using only these Rise-native block types:
Text | Image | Video | Quote | Statement | Numbered List | Bulleted List | Accordion | Tabs | Flashcards | Sorting | Labelled Graphic | Process | Timeline | Scenario | Knowledge Check | Button Stack | Divider

Output as a table:

| Section | Block Type | Purpose | Content Summary (1 line) | Interaction? |
|---------|-----------|---------|--------------------------|-------------|

Rules:
- No more than 2 consecutive Text blocks
- Every objective must be tested by at least one Knowledge Check
- Include at least one Scenario or Labelled Graphic per module
- Flag any section where a custom HTML embed would serve better than a native block
```

---

## Notes
- Run this before writing any content — it prevents the "wall of text" anti-pattern in Rise
- The flag for custom HTML embeds is useful when you're integrating Storyline blocks or interactive charts
- Pair with the Narration Script Writer for sections that use Statement or Process blocks
