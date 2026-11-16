# Prompt: Cognitive Load Audit

**Category:** Instructional Design  
**Target Tool:** Claude  
**Framework:** Role + Checklist + Structured Output  
**Use When:** Reviewing screen text, storyboard copy, or slide content before hand-off to development  
**Theory applied:** Cognitive Load Theory (#6) primary — Rationale: Working memory is limited; extraneous load from poor design directly reduces learning. Secondary: Cognitive Theory of Multimedia Learning (#10) — the redundancy, coherence, and signaling principles operationalize CLT for screen-based content.

---

## Prompt

```
You are a cognitive load specialist applying Sweller's Cognitive Load Theory and Mayer's Multimedia Learning Principles.

Audit the following eLearning content for cognitive load issues:

<content>
[PASTE SCREEN TEXT, NARRATION SCRIPT, OR STORYBOARD SECTION HERE]
</content>

Evaluate against these principles:
- Coherence (remove extraneous material that does not support the learning goal)
- Signaling (highlight key ideas so learners know what matters)
- Redundancy (avoid on-screen text that duplicates narration word-for-word)
- Spatial contiguity (related text and visuals must be placed together)
- Segmenting (content chunked into learner-paced steps, not one long stream)
- Modality (use narration + visuals rather than text + visuals where possible)

Output:
1. A severity-rated issue list (High / Medium / Low) with the specific text that triggers each issue and which principle it violates
2. A rewritten version of the content applying your fixes
3. One sentence explaining the most impactful change you made and why it reduces cognitive load

Reading level constraint: on-screen text must be Flesch-Kincaid Grade 8 or below; narration Grade 10 or below.
```

---

## Notes
- Best used on a single screen or 2–3 minute segment at a time — larger chunks degrade output quality
- "High" severity = likely causes learner confusion or drop-off; fix before development starts
- Combine with Bloom's Gap Analysis for a complete storyboard review pass
- For a full module audit, run this prompt screen-by-screen and log issues in a QA tracker
