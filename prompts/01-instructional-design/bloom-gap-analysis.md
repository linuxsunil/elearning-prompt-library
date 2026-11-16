# Prompt: Bloom's Taxonomy Gap Analysis

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Structured Output + Constraint  
**Use When:** Reviewing a course outline or learning objectives before development begins  
**Theory applied:** Bloom's Taxonomy Revised (#44) — Rationale: Cognitive level coverage directly determines whether the course develops recall, application, or higher-order thinking aligned to the performance goal.

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
2. A gap analysis — which levels are missing or over-represented relative to the stated performance goal
3. Three rewritten objectives that fill the most critical gaps, using measurable action verbs

Revised Bloom's verb rules:
- Remember: define, list, recall, recognize, identify, name
- Understand: explain, describe, summarize, classify, compare
- Apply: use, demonstrate, solve, execute, implement
- Analyze: differentiate, examine, deconstruct, attribute
- Evaluate: judge, critique, justify, recommend, assess
- Create: design, construct, produce, devise, formulate

Constraints:
- Flag any objectives using vague verbs (understand, know, appreciate) and suggest replacements
- No compound objectives — flag any using "and" to connect two verbs
- Assume a professional adult audience with no prior course experience
- Output in Markdown table format
```

---

## Notes
- Replace `[PASTE YOUR OUTLINE OR OBJECTIVES HERE]` with your actual content
- Works equally well with terminal objectives or enabling objectives
- Pair with the **Cognitive Load Audit** prompt after rewriting objectives
- For assessment alignment, follow up with: "Now map each rewritten objective to an assessment item type"
