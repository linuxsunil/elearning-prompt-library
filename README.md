# eLearning Prompt Library

> Production-ready AI prompts for Instructional Designers, eLearning Developers, and L&D Project Managers.

Built to work with [prompt-master](https://github.com/nidhinjs/prompt-master) — a Claude skill that optimises prompts for any AI tool.

---

## Why This Exists

Most AI prompts shared in the L&D community are vague. They produce generic output that still needs significant rework, wasting time and tokens.

This library applies proven prompt engineering principles — role assignment, structured output, constraints, few-shot examples, XML delimiters — specifically to eLearning workflows. Each prompt is designed to produce output you can use with minimal editing.

---

## Who This Is For

| Role | Most Useful Sections |
|------|---------------------|
| **Instructional Designer** | 01, 02, 04, 06 |
| **eLearning Developer** | 03, 07 |
| **L&D Project Manager** | 05, 06 |
| **Content Author** | 02, 04 |
| **L&D Team Lead** | All |

---

## Prompt Library

### 01 · Instructional Design
| Prompt | Purpose |
|--------|---------|
| [Bloom's Gap Analysis](prompts/01-instructional-design/bloom-gap-analysis.md) | Audit objectives for cognitive level coverage |
| [Cognitive Load Audit](prompts/01-instructional-design/cognitive-load-audit.md) | Review screen content against Mayer's principles |
| [SME Notes → Lesson Plan](prompts/01-instructional-design/sme-notes-to-lesson-plan.md) | Transform raw SME content using Merrill's First Principles |

### 02 · Content Development
| Prompt | Purpose |
|--------|---------|
| [Storyboard Shell Generator](prompts/02-content-development/storyboard-shell.md) | Scaffold a full module storyboard fast |
| [Narration Script Writer](prompts/02-content-development/narration-script-writer.md) | Convert notes to production narration (Ruth Colvin Clark style) |

### 03 · Storyline & Rise Development
| Prompt | Purpose |
|--------|---------|
| [Storyline Trigger & Variable Logic](prompts/03-storyline-rise/storyline-trigger-logic.md) | Design complex branching and variable architecture |
| [Rise Block Planner](prompts/03-storyline-rise/rise-block-planner.md) | Plan block sequences before building in Rise |
| [HTML5 Interaction Spec](prompts/03-storyline-rise/html5-interaction-spec.md) | Build accessible custom interactions for embedding |

### 04 · Assessment Design
| Prompt | Purpose |
|--------|---------|
| [Scenario-Based Assessment Designer](prompts/04-assessment/scenario-assessment-designer.md) | Write scenario questions that test application, not recall |
| [Question Bank Generator](prompts/04-assessment/question-bank-generator.md) | Build a full, Bloom's-mapped question bank |

### 05 · Project Management
| Prompt | Purpose |
|--------|---------|
| [Project Scoping & Timeline Estimator](prompts/05-project-management/project-scoping-estimator.md) | Estimate effort using Chapman's ratios + risk register |
| [Stakeholder Update Email](prompts/05-project-management/stakeholder-update-email.md) | Write clear RAG-status project updates |

### 06 · QA & Review
| Prompt | Purpose |
|--------|---------|
| [Storyboard QA Review](prompts/06-qa-review/storyboard-qa-checklist.md) | Multi-dimension storyboard review before development |
| [Published Course QA Checklist](prompts/06-qa-review/published-course-qa.md) | Pre-launch QA checklist with LMS-specific gotchas |

### 07 · AI Media
| Prompt | Purpose |
|--------|---------|
| [Midjourney eLearning Scenes](prompts/07-ai-media/midjourney-elearning-scene.md) | Generate course illustrations and character images |
| [ElevenLabs Voiceover Direction](prompts/07-ai-media/elevenlabs-voiceover-direction.md) | Configure AI narration for consistent module-wide voice |

---

## How to Use

### Option 1: With prompt-master (Recommended)

Install [prompt-master](https://github.com/nidhinjs/prompt-master) as a Claude skill, then invoke it with any prompt from this library as your starting point. The skill will further optimise the prompt for your specific tool and context.

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

### Option 3: Customise for your context

Add a **context block** at the top of any prompt to avoid repeating yourself:

```
<my_context>
I am an instructional designer at [COMPANY]. 
Our standard tool is Articulate Rise 360.
Our audience is always [AUDIENCE TYPE].
Our brand colours are [HEX CODES].
</my_context>
```

Paste this block before the prompt on every run.

---

## Prompt Design Principles

Every prompt in this library follows these rules:

- **Role assignment** — Claude performs better with an explicit expert persona
- **XML delimiters** — `<input>` tags separate your content from the instructions
- **Structured output** — numbered lists, tables, or defined sections — not open-ended prose
- **Constraints** — word limits, format rules, and "do not" instructions cut noise
- **Actionability** — output should be usable with minimal editing

---

## Contributing

Contributions welcome. Please follow the existing prompt format:

```markdown
# Prompt: [NAME]
**Category:** | **Target Tool:** | **Framework:** | **Use When:**
---
## Prompt
[THE ACTUAL PROMPT IN A CODE BLOCK]
---
## Notes
[3–5 practical tips]
```

---

## Built On

- [prompt-master](https://github.com/nidhinjs/prompt-master) by [@nidhinjs](https://github.com/nidhinjs) — the Claude skill that optimises these prompts
- Instructional design frameworks: Bloom's Taxonomy, Mayer's Multimedia Learning, Merrill's First Principles, Sweller's CLT, Ruth Colvin Clark
- Chapman's development ratio model for effort estimation

---

## License

MIT — use freely, attribution appreciated.
