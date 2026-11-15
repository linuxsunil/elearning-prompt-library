# Prompt: ElevenLabs Voiceover Direction

**Category:** AI Media  
**Target Tool:** ElevenLabs  
**Framework:** Voice Profile + SSML Guidance + Style Calibration  
**Use When:** Generating AI voiceover for eLearning narration with consistent tone across a module

---

## Voice Selection Guide

| Course Type | Recommended Voice Characteristics | Avoid |
|-------------|-----------------------------------|-------|
| Corporate compliance | Calm, authoritative, gender-neutral | Over-enthusiastic, sing-song |
| Leadership development | Warm, coaching, conversational | Stiff, monotone |
| Technical / IT skills | Clear, measured, precise | Fast, casual |
| Onboarding | Friendly, welcoming, energetic | Formal, distant |
| Safety training | Serious, direct, unhurried | Cheerful, light |

---

## ElevenLabs Settings Prompt

When generating narration in ElevenLabs, paste this in the **Style Exaggeration** and **Stability** notes (Projects tab):

```
Voice style: [coaching / professional / conversational — choose one]
Stability: 0.65 (consistent across a full module)
Similarity boost: 0.80
Style exaggeration: 0.20 (subtle — avoids over-acting)
Speaker boost: enabled

Delivery notes:
- Slight pause after each sentence (the script uses full stops as breath cues)
- Emphasis words are marked in [brackets] — slightly stress these
- Questions should end with a natural upward inflection
- Do not speed up at the end of long sentences
```

---

## Script Formatting for Best Results

```
[Normal sentence delivered at a measured pace.]

[KEY TERM] — this term should receive slight emphasis.

Pause here... [use ellipsis for half-beat pause]

[Long complex sentence — break with a comma, like this, to signal natural breath.]
```

---

## Notes
- Regenerate any sentence that sounds rushed — ElevenLabs is inconsistent on first generation
- For multi-module projects, save your voice settings as a "Project" in ElevenLabs to ensure consistency
- Download as MP3 at 128kbps for Rise; WAV for Storyline (better sync with timeline)
