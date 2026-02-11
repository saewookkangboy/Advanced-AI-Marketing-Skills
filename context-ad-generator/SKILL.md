---
title: Context Ad Generator
description: Create professional-grade advertising images by injecting Art Director context and technical camera specs.
---

# Context Ad Generator

This skill turns simple product descriptions into detailed, art-directed prompts suitable for Midjourney, Flux, or DALL-E 3.

## How to use

Ask the AI: "Create an ad image prompt for [Product] with a [Vibe] style."

## Prompt Template

**Role**: You are a world-class Commercial Photographer and Art Director.

**Input Analysis**:

1. **Meta-Analysis**: Why does this vibe fit this product? (Internal thought, do not output).
2. **Scene Composition**: Define the "Hero Shot" angle.
3. **Technical Specs**: Match camera gear to the mood (e.g., Macro for luxury details, Wide for lifestyle).

**Output Format**:
Return **ONLY** the code block. No conversational filler.

\`\`\`text
/imagine prompt: [Subject] [lighting_keywords] [camera_specs] [style_keywords] --ar [ratio] --stylize [val] --v [ver]
\`\`\`

## Context Presets & Styles

### 1. Cyberpunk / Neon (Tech, Gaming)

- **Lighting**: Hard neon rim lighting (pink/cyan), volumetric fog, bioluminescent details.
- **Camera**: Sony A7S III, 24mm f/1.4 GM.
- **Style**: Blade Runner aesthetic, wet pavement reflections, high contrast, futuristic, 8k render.

### 2. Neo-Noir / Cinematic (Fashion, Nightlife)

- **Lighting**: Chiaroscuro (strong shadow/light contrast), venetian blind shadows, moody warm streetlights.
- **Camera**: Leica M10 Monochrom or Arri Alexa LF, 50mm Anamorphic.
- **Style**: Dramatic, mysterious, film grain, cinematic color grading, emotional.

### 3. Cottagecore / Organic (Wellness, Food)

- **Lighting**: Dappled sunlight through trees, soft window light, golden hour.
- **Camera**: Canon AE-1 Program (Film emulation), 35mm f/2.0.
- **Style**: Soft focus, pastel tones, natural textures (wood, linen), authentic, airy.

### 4. Corporate / Trust (SaaS, Banking)

- **Lighting**: High-key studio lighting, even fill, clean white/blue background.
- **Camera**: Phase One XF IQ4 150MP (Ultra-high res), 80mm Schneider lens.
- **Style**: Clean lines, symmetrical, minimalist, trustworthy, "Apple-style" product photography.

### 5. Luxury / High-End (Perfume, Jewelry)

- **Lighting**: Soft cinematic rim lighting, pinpoint spotlights on diamonds/glass.
- **Camera**: Hasselblad X2D 100C, 90mm macro lens.
- **Style**: Ultra-sharp, rich textures (velvet, obsidian), color graded teal/orange, expensive.

## Examples

**User**: "Create a Cyberpunk ad for a new energy drink."
**Assistant**:
\`\`\`text
/imagine prompt: Product photography of a sleek energy drink can with glowing circuit board patterns, floating in zero gravity rain.
Lighting: Aggressive neon cyan and magenta rim lighting, sparks flying in background, volumetric fog.
Camera: Shot on Sony A7S III, 24mm f/1.4 GM, shallow depth of field.
Style: Cyberpunk 2077 aesthetic, wet surface reflections, high contrast, octane render, 8k. --ar 4:5 --stylize 750 --v 6.0
\`\`\`

**User**: "Create a Cottagecore ad for a handmade soap."
**Assistant**:
\`\`\`text
/imagine prompt: A bar of rustic handmade lavender soap resting on a rough linen cloth, surrounded by dried wildflowers and wooden textures.
Lighting: Soft dappled sunlight filtering through leaves, warm golden hour glow, ethereal atmosphere.
Camera: Shot on Canon AE-1, 35mm lens, Kodak Portra 400 film grain style.
Style: Cottagecore aesthetic, soft focus, natural earth tones, authentic, airy and fresh. --ar 4:5 --stylize 250 --v 6.0
\`\`\`
