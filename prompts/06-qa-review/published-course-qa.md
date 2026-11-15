# Prompt: Published Course QA Checklist Generator

**Category:** QA & Review  
**Target Tool:** Claude  
**Framework:** Role + Checklist + Tool-Specific  
**Use When:** Preparing for final QA before publishing a course to the LMS

---

## Prompt

```
You are an eLearning QA specialist. Generate a comprehensive QA checklist for a course about to be published.

Course details:
- Authoring tool: [Articulate Rise 360 / Storyline 360 / Custom HTML]
- LMS: [Moodle / Cornerstone / SAP SuccessFactors / CSOD / Docebo / Other]
- SCORM version: [SCORM 1.2 / SCORM 2004 / xAPI / AICC]
- Completion trigger: [Quiz score / Slide viewed / Time spent / Custom variable]
- Has audio: [Yes / No]
- Has video: [Yes / No]
- Has branching: [Yes / No]
- Accessibility requirement: [WCAG 2.1 AA / Section 508 / None]
- Target devices: [Desktop only / Desktop + Mobile / All devices]

Generate a checklist covering:
1. Content accuracy (5 items)
2. Functionality — navigation, buttons, triggers (8 items)
3. SCORM/xAPI tracking — completion, score, resume (6 items)
4. Media — audio sync, video playback, captions (5 items)
5. Accessibility — keyboard nav, screen reader, contrast (6 items)
6. Cross-browser/device testing matrix (table format)
7. LMS-specific gotchas for [LMS NAME] (3–5 items)

Format as a checklist with checkboxes [ ] and severity label (Critical / Standard) for each item.
```

---

## Notes
- LMS-specific gotchas are often the most valuable output — they catch the issues that waste hours post-launch
- Run this before every publish, not just the first one — re-publishing after edits can reset SCORM tracking
- For xAPI: add "Verify statement actors match LMS user IDs" to the tracking section
