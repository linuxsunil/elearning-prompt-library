# Contributing to the eLearning Prompt Library

Thank you for contributing. This library stays useful only if prompts are genuinely production-tested.

## What Makes a Good Contribution

✅ Prompts you've actually used on a real project  
✅ Prompts that produce output needing minimal editing  
✅ Prompts that are specific to eLearning workflows (not generic writing tasks)  
✅ Clear placeholders in `[BRACKETS]` for every variable input  

❌ Prompts copied from other libraries without testing  
❌ Overly general prompts ("write me a quiz")  
❌ Prompts that only work with one very specific LMS or tool  

## Prompt Format

Every prompt file must follow this structure:

```markdown
# Prompt: [DESCRIPTIVE NAME]

**Category:** [Category folder name]  
**Target Tool:** [Claude / Claude Code / Midjourney / ElevenLabs / etc.]  
**Framework:** [The prompt technique(s) used]  
**Use When:** [One sentence — when should someone reach for this prompt?]

---

## Prompt

\```
[THE EXACT PROMPT TEXT]
\```

---

## Notes
- [Practical tip 1]
- [Practical tip 2]
- [Practical tip 3]
```

## Category Folders

| Folder | Contents |
|--------|---------|
| `01-instructional-design` | Objectives, curriculum design, learning theory application |
| `02-content-development` | Storyboards, scripts, content writing |
| `03-storyline-rise` | Articulate-specific prompts, HTML5 interactions |
| `04-assessment` | Questions, scenarios, rubrics |
| `05-project-management` | Scoping, timelines, stakeholder comms |
| `06-qa-review` | Quality review, testing, accessibility |
| `07-ai-media` | Midjourney, ElevenLabs, Sora, DALL-E |

New categories welcome — open an issue first to discuss.

## Submitting

1. Fork the repo
2. Create a branch: `git checkout -b prompt/your-prompt-name`
3. Add your prompt file in the correct folder
4. Update `README.md` to add a row in the relevant table
5. Open a PR with a one-line description of what the prompt does

## Questions

Open an issue with the `question` label.
