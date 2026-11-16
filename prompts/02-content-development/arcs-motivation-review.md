# Prompt: ARCS Motivation Review

**Category:** Content Development  
**Target Tool:** Claude  
**Framework:** Role + Keller's ARCS Model + Structured Output  
**Use When:** A course exists but learners are disengaged, dropping off, or not completing — or when designing for a known low-motivation audience  
**Theory applied:** ARCS Model (#35) primary — Rationale: Keller's four categories (Attention, Relevance, Confidence, Satisfaction) provide a systematic framework for diagnosing and fixing motivation gaps in any course. Secondary: Self-Determination Theory (#27) — autonomy, competence, and relatedness explain the deeper psychological needs that ARCS strategies address.

---

## Prompt

```
You are an instructional designer specializing in learner motivation, applying Keller's ARCS Model.

Review the following course content or design for motivation issues and recommend improvements:

<content>
[PASTE COURSE OUTLINE, STORYBOARD, OR MODULE DESCRIPTION HERE]
</content>

Audience context:
- Who are the learners: [ROLE, EXPERIENCE LEVEL]
- Known motivation challenge: [e.g., compliance course nobody wants to take / advanced topic for resistant audience / self-paced course with high drop-off]
- Delivery format: [eLearning / ILT / Blended]

Evaluate against all four ARCS categories:

**A — Attention**
- Does the course open with a hook (scenario, surprising statistic, provocative question)?
- Is there variety in content format to maintain attention throughout?
- Are there inquiry-arousing activities (what do you think happens if...)?

**R — Relevance**
- Is the connection to the learner's job made explicit in the first screen?
- Are examples drawn from the learner's real work context?
- Does the course acknowledge what learners already know and can do?

**C — Confidence**
- Is difficulty scaffolded (easy wins first, then increasing challenge)?
- Do learners know what success looks like before they are assessed?
- Is feedback encouraging without being dishonest?

**S — Satisfaction**
- Do learners receive a sense of accomplishment at the end?
- Is there a job aid, certificate, or next-step resource to take away?
- Does completing the course lead to something the learner values?

Output:
1. ARCS gap analysis — which categories are weak and why (with specific evidence from the content)
2. Five concrete design recommendations, one per ARCS category plus one for the opening hook
3. A revised opening screen (hook + objective display + relevance statement) — ready to paste into a storyboard
```

---

## Notes
- Low completion rates usually trace to weak R (Relevance) — learners don't see why this matters to them
- Compliance courses most often fail on A (Attention) and S (Satisfaction) — they open with policy and end with "quiz passed"
- For ILT: the same ARCS analysis applies to session design — facilitator energy covers Attention but Relevance and Satisfaction need explicit design
- Pair with the SME Notes → Lesson Plan prompt to rebuild the structure after diagnosis
