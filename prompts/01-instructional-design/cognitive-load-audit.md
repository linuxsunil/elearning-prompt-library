# Prompt: Cognitive Load Audit

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Checklist + Structured Output  
**Use When:** Reviewing screen text, storyboard copy, or slide content before hand-off to development

---

## Prompt

```
You are a cognitive load specialist applying Sweller's Cognitive Load Theory and Mayer's Multimedia Learning Principles.

Audit the following eLearning content for cognitive load issues:

<content>
[PASTE SCREEN TEXT, NARRATION SCRIPT, OR STORYBOARD SECTION HERE]
</content>

Evaluate against these principles:
- Coherence (remove extraneous material)
- Signaling (highlight key ideas)
- Redundancy (avoid on-screen text that duplicates narration word-for-word)
- Spatial contiguity (related text and visuals placed together)
- Segmenting (content chunked into learner-paced steps)

Output:
1. A severity-rated issue list (High / Medium / Low) with the specific text that triggers each issue
2. A rewritten version of the content applying your fixes
3. One sentence explaining the most impactful change you made
```

---

## Notes
- Best used on a single screen or 2–3 minute segment at a time
- "High" severity = likely causes learner confusion or drop-off
- Combine with Bloom's Gap Analysis for a complete storyboard review pass
