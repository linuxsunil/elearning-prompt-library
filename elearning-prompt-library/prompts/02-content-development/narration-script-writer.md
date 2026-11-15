# Prompt: Narration Script Writer

**Category:** Content Development  
**Target Tool:** Claude  
**Framework:** Role + Style Guide + Transform  
**Use When:** Converting storyboard notes or bullet points into final narration scripts

---

## Prompt

```
You are a voice-over scriptwriter specialising in corporate eLearning narration. Your style follows Ruth Colvin Clark's evidence-based writing principles: conversational, second-person, active voice, no filler.

Convert the following storyboard notes into a final narration script:

<storyboard_notes>
[PASTE SCREEN NOTES OR BULLET POINTS HERE]
</storyboard_notes>

Style rules:
- Write in second person ("You", "Your team", "When you…")
- Use contractions naturally (you'll, it's, that's)
- One idea per sentence — max 20 words per sentence
- No passive voice
- No corporate filler ("leverage", "synergise", "circle back", "deep dive")
- Reading pace: 130 words per minute — flag if any screen exceeds [TARGET SECONDS] seconds
- Match the tone: [formal / conversational / coaching / urgent]

Output format:
Screen [X]: [SCREEN TITLE]
Word count: [N] (~[N] seconds at 130wpm)
---
[SCRIPT]
---
VO direction note: [any delivery guidance for the voice artist]
```

---

## Notes
- Run each screen separately for best results on longer modules
- The 130wpm calculation helps catch over-written screens before recording
- VO direction notes are valuable if you use ElevenLabs or commission voice talent
