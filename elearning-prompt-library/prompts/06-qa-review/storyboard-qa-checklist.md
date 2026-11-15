# Prompt: Storyboard QA Review

**Category:** QA & Review  
**Target Tool:** Claude  
**Framework:** Role + Multi-Dimension Review + Severity Rating  
**Use When:** Reviewing a completed storyboard before it goes to development

---

## Prompt

```
You are a senior instructional designer performing a quality review of an eLearning storyboard.

Review the following storyboard for quality issues:

<storyboard>
[PASTE STORYBOARD CONTENT — can be a table, bullet points, or screen-by-screen notes]
</storyboard>

Module context:
- Audience: [WHO]
- Learning objectives: [LIST THEM]
- Delivery tool: [Rise / Storyline / Other]

Review across these six dimensions and rate each issue (Critical / Major / Minor):

1. **Instructional integrity** — do activities align with stated objectives? Are higher-order objectives tested, not just recalled?
2. **Cognitive load** — any screens that overload working memory? Text-heavy screens, missing chunking?
3. **Narration quality** — passive voice, jargon, filler words, redundancy with on-screen text?
4. **Engagement** — are there at least 2 non-quiz interactions per 10 minutes of content?
5. **Accessibility red flags** — anything that would fail WCAG 2.1 AA (colour-only information, missing alt text notes, autoplay media)?
6. **Development feasibility** — any requests that are technically unrealistic for the stated tool?

Output a numbered issue list with: Dimension | Screen # | Severity | Issue description | Suggested fix

End with: "X Critical issues must be resolved before development begins."
```

---

## Notes
- Critical issues = block development; Major = resolve in first dev review; Minor = nice-to-have
- For large storyboards (20+ screens), review in sections of 10 screens for best output quality
- Save the issue list as a comment in your project tracker for accountability
