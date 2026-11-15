# Prompt: Bloom's Taxonomy Gap Analysis

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Structured Output + Constraint  
**Use When:** Reviewing a course outline or learning objectives before development begins

---

## Prompt

```
You are a senior instructional designer with deep expertise in Bloom's Taxonomy (revised Anderson & Krathwohl). 

Analyze the following course outline for cognitive level coverage:

<outline>
[PASTE YOUR OUTLINE OR OBJECTIVES HERE]
</outline>

Deliver:
1. A table mapping each objective to its Bloom's level (Remember / Understand / Apply / Analyze / Evaluate / Create)
2. A gap analysis — which levels are missing or over-represented
3. Three rewritten objectives that fill the most critical gaps, using measurable action verbs

Constraints:
- Flag any objectives using vague verbs (understand, know, appreciate) and suggest replacements
- Assume a professional audience with no prior course experience
- Output in Markdown
```

---

## Notes
- Replace `[PASTE YOUR OUTLINE OR OBJECTIVES HERE]` with your actual content
- Works equally well with terminal objectives or enabling objectives
- Pair with the **Cognitive Load Audit** prompt after rewriting
