# Prompt: UDL Accessibility Audit

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + UDL Three Principles + WCAG 2.1 AA  
**Use When:** Auditing a module design or storyboard for inclusive design — before development or as part of QA  
**Theory applied:** Universal Design for Learning (#51) primary — Rationale: UDL's three principles (multiple means of representation, action/expression, and engagement) ensure content is accessible to learners with different abilities, learning preferences, and contexts before technical WCAG fixes are needed. Secondary: Andragogy (#28) — adult learners require multiple pathways to engage with content on their own terms.

---

## Prompt

```
You are an inclusive learning design specialist applying Universal Design for Learning (UDL) and WCAG 2.1 AA standards.

Audit the following course design or storyboard for inclusive design issues:

<design>
[PASTE STORYBOARD, MODULE OUTLINE, OR SCREEN DESCRIPTIONS HERE]
</design>

Module context:
- Delivery tool: [Articulate Rise / Storyline 360 / Custom HTML]
- Known accessibility requirements: [WCAG 2.1 AA / Section 508 / client-specific]
- Known audience diversity: [any known disability, language, device, or bandwidth considerations]

Evaluate across UDL's three principles:

**Principle 1 — Multiple Means of Representation (the "what" of learning)**
- Is information presented in more than one format (text + audio + visual)?
- Are key concepts explained with examples, analogies, or diagrams?
- Is background knowledge activated before new content is introduced?
- Are language and vocabulary accessible (FK Grade 10 or below for narration)?

**Principle 2 — Multiple Means of Action and Expression (the "how" of learning)**
- Can learners navigate and interact using keyboard only?
- Are there alternative ways to demonstrate learning beyond MCQ?
- Are timed activities avoidable or extendable?
- Is there a text alternative for any audio or video content?

**Principle 3 — Multiple Means of Engagement (the "why" of learning)**
- Is the relevance to the learner's job made explicit?
- Are there options for self-assessment or reflection?
- Is the difficulty scaffolded (not all hard, not all easy)?
- Are diverse learner contexts, names, and scenarios represented?

**WCAG 2.1 AA technical flags**
- Colour contrast: text minimum 4.5:1, large text 3:1
- No colour-only information encoding
- All meaningful images require alt text notes
- All video requires a caption file
- Focus indicators visible on all interactive elements

Output: a prioritised issue list (Critical / Major / Minor) with suggested fixes.
End with: a one-paragraph UDL design recommendation for the developer.
```

---

## Notes
- Run this after the Storyboard QA Review for a complete pre-development quality pass
- UDL and WCAG overlap but are not the same — WCAG is technical compliance; UDL is proactive inclusive design
- For Rise: check that all Accordion, Tab, and Flashcard blocks are keyboard accessible before publishing
- For Storyline: check tab order on every slide with interactions (Object → Tab Order in the ribbon)
