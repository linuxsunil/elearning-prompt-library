# Prompt: Standalone HTML5 Interaction Spec (Claude Code)

**Category:** Storyline / Rise Development  
**Target Tool:** Claude Code  
**Framework:** Role + Spec + WCAG Constraint  
**Use When:** Building a custom HTML5 interaction to embed in Rise or Storyline via web object

---

## Prompt

```
You are a front-end developer building accessible eLearning interactions.

Build a standalone HTML5 interaction with the following specification:

<spec>
Interaction type: [e.g., drag-and-drop matching / clickable hotspot / accordion / card flip / branching mini-scenario]
Content: [DESCRIBE WHAT THE LEARNER DOES AND WHAT FEEDBACK THEY RECEIVE]
Data: [PASTE THE ACTUAL CONTENT — labels, options, correct answers, feedback text]
Embedding target: [Articulate Rise web object / Storyline web object / standalone browser]
</spec>

Requirements:
- Single self-contained HTML file (HTML + CSS + JS, no external CDN dependencies)
- WCAG 2.1 AA compliant (keyboard navigable, ARIA labels, sufficient colour contrast)
- Mobile responsive (works at 320px minimum width)
- Completion signal: postMessage to parent when learner completes (for Rise/Storyline integration)
- No frameworks — vanilla JS only
- Colour scheme: [PASTE HEX CODES or "use a neutral corporate palette"]

Deliver:
1. The complete HTML file
2. A 5-item QA checklist specific to this interaction
3. The postMessage payload format used for completion
```

---

## Notes
- The postMessage requirement is what allows Rise to track completion of embedded web objects
- "No CDN dependencies" is critical — LMS environments often block external requests
- For Storyline embedding: set the web object to "Load automatically" and check "Allow internet access"
