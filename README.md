# eLearning Prompt Library

> Production-ready AI prompts for Instructional Designers, eLearning Developers, and L&D Project Managers.  
> Every prompt is grounded in a specific learning theory from the [60-theory reference library](INSTRUCTIONAL-DESIGN-FOUNDATIONS.md).

Built to work with [prompt-master](https://github.com/nidhinjs/prompt-master) — a Claude skill that optimizes prompts for any AI tool.

---

## Why This Exists

Most AI prompts shared in the L&D community are vague. They produce generic output that needs significant rework, wasting time and tokens. And they don't cite *why* a prompt is structured the way it is.

This library applies proven prompt engineering techniques — role assignment, structured output, XML delimiters, format constraints — specifically to eLearning workflows. Each prompt cites the learning theory or ID model that shapes it, so you can adapt it intelligently for your own context.

---

## Theoretical Foundation

Every prompt includes a **Theory applied** line:

```
Theory applied: [Name] (#Number) — Rationale: [one sentence]
```

The number maps to the full [Instructional Design Foundations](INSTRUCTIONAL-DESIGN-FOUNDATIONS.md) reference — 60 theories across behavioural, cognitive, constructivist, humanistic, connectivist, and motivation frameworks, with a selection guide, Bloom's verb map, Gagné event reference, and assessment quality rules.

---

## Who This Is For

| Role | Most Useful Sections |
|------|---------------------|
| **Instructional Designer** | 01, 02, 04, 06 |
| **eLearning Developer** | 03, 07 |
| **L&D Project Manager** | 05, 06 |
| **Content Author** | 02, 04 |
| **L&D Team Lead / LX Designer** | All |

---

## Prompt Library

### 01 · Instructional Design

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Theory Selector](prompts/01-instructional-design/theory-selector.md) | All 60 theories | Pick the right primary + secondary theory for any brief |
| [Bloom's Gap Analysis](prompts/01-instructional-design/bloom-gap-analysis.md) | Bloom's Revised (#44) | Audit objectives for cognitive level coverage |
| [Cognitive Load Audit](prompts/01-instructional-design/cognitive-load-audit.md) | CLT (#6) + Mayer (#10) | Review screen content against multimedia learning principles |
| [SME Notes → Lesson Plan](prompts/01-instructional-design/sme-notes-to-lesson-plan.md) | Merrill's (#45) + Andragogy (#28) | Transform raw SME content into a structured lesson plan |
| [Gagné Module Planner](prompts/01-instructional-design/gagne-module-planner.md) | Gagné's Nine Events (#43) | Plan a module's full instructional sequence |
| [Action Mapping](prompts/01-instructional-design/action-mapping.md) | Action Mapping (#50) + Operant Conditioning (#2) | Determine whether training is the right solution before building |
| [UDL Accessibility Audit](prompts/01-instructional-design/udl-accessibility-audit.md) | UDL (#51) + Andragogy (#28) | Audit for inclusive design before development |

### 02 · Content Development

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Storyboard Shell Generator](prompts/02-content-development/storyboard-shell.md) | Gagné (#43) + Info Processing (#8) | Scaffold a full module storyboard fast |
| [Narration Script Writer](prompts/02-content-development/narration-script-writer.md) | Mayer (#10) + Andragogy (#28) | Convert notes to production narration |
| [ARCS Motivation Review](prompts/02-content-development/arcs-motivation-review.md) | ARCS (#35) + SDT (#27) | Diagnose and fix engagement and motivation gaps |

### 03 · Storyline & Rise Development

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Storyline Trigger & Variable Logic](prompts/03-storyline-rise/storyline-trigger-logic.md) | — | Design complex branching and variable architecture |
| [Rise Block Planner](prompts/03-storyline-rise/rise-block-planner.md) | Info Processing (#8) | Plan block sequences before building in Rise |
| [HTML5 Interaction Spec](prompts/03-storyline-rise/html5-interaction-spec.md) | UDL (#51) | Build accessible custom interactions for embedding |

### 04 · Assessment Design

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Scenario-Based Assessment Designer](prompts/04-assessment/scenario-assessment-designer.md) | Situated Learning (#20) + Retrieval Practice (#54) | Write scenario questions that test application, not recall |
| [Question Bank Generator](prompts/04-assessment/question-bank-generator.md) | Retrieval Practice (#54) + Interleaving (#53) | Build a full Bloom's-mapped question bank |
| [Kirkpatrick Evaluation Plan](prompts/04-assessment/kirkpatrick-evaluation-plan.md) | Kirkpatrick (#48) + Phillips ROI (#49) | Design a four-level evaluation strategy |

### 05 · Project Management

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Project Scoping & Timeline Estimator](prompts/05-project-management/project-scoping-estimator.md) | ADDIE (#41) + SAM (#42) | Estimate effort using Chapman's ratios + risk register |
| [Stakeholder Update Email](prompts/05-project-management/stakeholder-update-email.md) | — | Write clear RAG-status project updates |

### 06 · QA & Review

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Storyboard QA Review](prompts/06-qa-review/storyboard-qa-checklist.md) | CLT (#6) + Gagné (#43) | Multi-dimension storyboard review before development |
| [Published Course QA Checklist](prompts/06-qa-review/published-course-qa.md) | UDL (#51) | Pre-launch QA checklist with LMS-specific gotchas |

### 07 · AI Media

| Prompt | Theory | Purpose |
|--------|--------|---------|
| [Midjourney eLearning Scenes](prompts/07-ai-media/midjourney-elearning-scene.md) | Dual Coding (#9) | Generate course illustrations and character images |
| [ElevenLabs Voiceover Direction](prompts/07-ai-media/elevenlabs-voiceover-direction.md) | Mayer (#10) | Configure AI narration for consistent module-wide voice |

---

## How to Use

### Option 1: With prompt-master (Recommended)

Install [prompt-master](https://github.com/nidhinjs/prompt-master) as a Claude skill, then invoke it with any prompt from this library as your starting point.

```bash
# Claude Code (CLI)
git clone https://github.com/nidhinjs/prompt-master ~/.claude/skills/prompt-master
```

Then in Claude Code:
```
/prompt-master [paste any prompt from this library]
```

### Option 2: Direct use

Copy any prompt, fill in the `[BRACKETED PLACEHOLDERS]`, and paste into Claude, ChatGPT, or any AI tool.

### Option 3: Add a context block

Avoid repeating yourself across prompts by prepending a context block:

```
<my_context>
I am an instructional designer at [COMPANY].
Our standard authoring tool is Articulate Rise 360.
Our audience is always [AUDIENCE TYPE] — adult professionals.
Our brand colors are [HEX CODES].
Default to American English.
</my_context>
```

### Option 4: Run the Theory Selector first

For any new module, run the **Theory Selector** prompt before writing a single word of content. It outputs a primary and secondary theory recommendation with rationale — paste that into every downstream prompt to keep the design coherent.

---

## Workflow: Full Module From Scratch

```
1. Theory Selector          → choose primary + secondary theory
2. Action Mapping           → validate that training is the right solution
3. Gagné Module Planner     → map the instructional sequence
4. SME Notes → Lesson Plan  → structure the content
5. Bloom's Gap Analysis     → verify objectives are at the right cognitive level
6. Storyboard Shell         → scaffold the full module
7. Narration Script Writer  → write screen-by-screen narration
8. ARCS Motivation Review   → check engagement design
9. Scenario Assessment      → design the practice activities
10. Question Bank Generator → build the summative assessment
11. UDL Audit               → check for inclusive design issues
12. Storyboard QA Review    → final check before development
```

---

## Prompt Design Principles

Every prompt in this library follows these rules:

- **Theory citation** — `Theory applied:` line states which of the 60 theories shapes the prompt
- **Role assignment** — Claude performs better with an explicit expert persona
- **XML delimiters** — `<input>` tags separate your content from the instructions
- **Structured output** — tables, numbered lists, or defined sections — not open-ended prose
- **Constraints** — word limits, format rules, and "do not" instructions cut noise
- **Actionability** — output is usable with minimal editing

---

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the prompt format and submission process.

Each prompt must:
- Cite at least one theory from [INSTRUCTIONAL-DESIGN-FOUNDATIONS.md](INSTRUCTIONAL-DESIGN-FOUNDATIONS.md)
- Follow the standard prompt format
- Have been tested on a real project before submission

---

## Built On

- [prompt-master](https://github.com/nidhinjs/prompt-master) by [@nidhinjs](https://github.com/nidhinjs) — the Claude skill that optimizes these prompts
- 60 learning theories and ID models documented in [INSTRUCTIONAL-DESIGN-FOUNDATIONS.md](INSTRUCTIONAL-DESIGN-FOUNDATIONS.md)
- Chapman's development ratio model for effort estimation
- Cathy Moore's Action Mapping methodology
- Ruth Colvin Clark's evidence-based writing principles

---

## License

MIT — use freely, attribution appreciated.
