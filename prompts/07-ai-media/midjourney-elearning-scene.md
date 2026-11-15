# Prompt: Midjourney eLearning Scene

**Category:** AI Media  
**Target Tool:** Midjourney  
**Framework:** Subject + Style + Technical Params  
**Use When:** Generating custom illustration or photography-style images for eLearning modules

---

## Prompt Templates

### Corporate scenario scene
```
/imagine [SCENE DESCRIPTION], diverse professional team, modern open-plan office, natural lighting, candid moment, editorial photography style, Sony A7 85mm f/1.8, shallow depth of field, warm neutral tones, no text, no logos --ar 16:9 --style raw --v 6.1
```

### Character portrait (for scenario personas)
```
/imagine professional headshot of [DEMOGRAPHIC — e.g., South Asian woman in her 30s], business casual, confident expression, neutral studio background, soft lighting, editorial portrait photography, Canon 5D 50mm --ar 1:1 --style raw --v 6.1
```

### Abstract concept illustration
```
/imagine [CONCEPT — e.g., data privacy, teamwork, compliance], flat design illustration, clean geometric shapes, [BRAND COLOUR HEX e.g., #0057B8] and white palette, minimal, corporate, svg-style, no gradients --ar 16:9 --v 6.1
```

### Process / infographic visual
```
/imagine [PROCESS — e.g., 5-step onboarding flow], isometric flat illustration, numbered steps, clean icons, light background, modern corporate style, no text --ar 16:9 --v 6.1
```

---

## Tips
- Always add `no text, no logos` to avoid unusable watermarks or hallucinated text
- Use `--ar 16:9` for slide backgrounds, `--ar 4:3` for Rise image blocks, `--ar 1:1` for personas
- For character consistency across scenes: generate a character sheet first with `--cref` in v6.1
- Replace `[BRAND COLOUR HEX]` with your actual brand colour for consistent visual identity
- Add `--no hands` if Midjourney keeps generating distorted hands in close-up scenes
