# ComfyUI Prompt Library — Dark Shonen Style

**Model: Flux 2 Klein (9B) — Qwen3 Text Encoder**
Companion to the Visual Style Bible v1.0 — March 2026

---

## How to Use This Document

Flux 2 Klein uses a **Qwen3 language model** as its text encoder. Unlike SDXL/CLIP-based models, it understands natural language — full sentences, spatial relationships, and context. This changes everything about how you write prompts.

### Key Rules for Flux 2 Klein

- **Write in natural language.** Describe scenes as if you're explaining a painting to someone. No comma-separated tag lists.
- **Subject first.** Flux weighs earlier tokens more heavily. Always start with *what* the image is, then build outward.
- **No negative prompts.** Flux does not support them. Describe what you *want*, never what you don't.
- **No prompt weights.** Syntax like `(tag:1.2)` does nothing. Use emphasis phrases instead: "with particular emphasis on the eyes" or "the most prominent feature is the scar across his jaw."
- **No quality tags.** "Masterpiece, best quality, highly detailed" are SDXL artifacts. Flux ignores them. Describe the actual visual qualities you want instead.
- **Be spatially specific.** Describe foreground, midground, background. Flux handles layered compositions well.
- **Keep it concise but descriptive.** 2-4 sentences is the sweet spot. Overly long prompts dilute focus.

### Prompt Structure

Every prompt follows this hierarchy:

> **Subject** → **Action/Pose** → **Appearance Details** → **Environment** → **Lighting** → **Style/Mood**

### Recommended ComfyUI Settings

| Parameter | Value |
|-----------|-------|
| Steps | 4 (distilled) or 20-30 (base) |
| CFG / Guidance | 1.0 (distilled) or 3.0-4.5 (base) |
| Resolution | 1024×1024, or 768×1344 for portraits |
| Sampler | Euler (distilled) or DPM++ 2M (base) |

---

## 1. Style Anchors

These opening phrases set the visual language. **Always start your prompt with one of these**, then continue with your subject description.

### General Purpose

> A dark fantasy anime illustration in a shonen manga style, with visible ink linework, rich saturated colors emerging from deep blacks, and dramatic atmospheric lighting.

### Character Portrait

> A dark fantasy anime character portrait in the style of shonen manga, featuring detailed ink outlines, expressive eyes with light reflections, dramatic chiaroscuro lighting, and rich colors against deep shadows.

### Environment / Landscape

> A dark fantasy anime landscape illustration with detailed background art, visible ink linework in the foreground, atmospheric perspective fading into deep shadow, volumetric lighting, and rich saturated colors.

### Creature / Bestiary

> A dark fantasy anime creature illustration in a shonen manga style, with detailed ink outlines, textured anatomy, dramatic lighting from a single source, and rich colors punching through deep blacks.

---

## 2. Character Pre-Prompts

Each entry below is a complete, ready-to-use prompt. Replace the `[BRACKETED]` sections with your specifics.

---

### Humans — Civilized

> A dark fantasy anime character portrait in shonen manga style with visible ink outlines and dramatic chiaroscuro lighting. A [male/female] human warrior stands in a confident pose, shown from the chest up. They have [HAIR COLOR] hair and [EYE COLOR] eyes with detailed reflections. They wear ornate crafted armor over embroidered fabric, with warm amber and gold tones throughout their design. The background is dark and atmospheric, with rim lighting catching the edges of their figure and a faint wind moving their hair. Their expression is calm and assured. [WEAPON OR ACCESSORY DESCRIPTION].

### Humans — Barbarian

> A dark fantasy anime character portrait in shonen manga style with bold ink outlines and harsh dramatic side lighting. A [male/female] human barbarian is shown from the chest up, with wild unkempt [HAIR COLOR] hair and fierce [EYE COLOR] eyes. Their build is muscular and weathered, wearing fur pelts and rough leather armor. Tribal tattoos mark their skin and a battle scar crosses their [face/arm/chest]. The color palette is cold — steel blues, greys, and whites — with snow particles drifting in the air. The background is a dark stormy sky. Their expression is fierce and determined. [WEAPON OR ACCESSORY DESCRIPTION].

### Humans — Primitive

> A dark fantasy anime character portrait in shonen manga style with visible ink linework and warm dappled sunlight filtering through a jungle canopy. A [male/female] human from a primitive tribe is shown from the chest up. They have [HAIR COLOR] hair adorned with feathers and beads, and alert [EYE COLOR] eyes. Their lean, wiry body is dressed in bone and leather tribal gear, with ritualistic body paint in geometric patterns. The color palette is earthy — forest greens, ochres, and deep browns. Their expression is primal and watchful. [WEAPON OR ACCESSORY DESCRIPTION].

---

### Elf

> A dark fantasy anime character portrait in shonen manga style with elegant ink outlines and cold moonlight filtering through a dark forest canopy. An [male/female] elf is shown from the chest up, with long pointed ears that extend well beyond their hair. Their facial features are angular and sharp, with luminous almond-shaped [EYE COLOR] eyes. Their [HAIR COLOR] hair flows long and straight. They wear flowing organic robes with subtle leaf and vine motifs, in silver and violet tones. Their posture carries a subtle air of ancient superiority. The background is a dark mystical forest with an ethereal, otherworldly atmosphere. Their expression is serene but distant.

### Dwarf

> A dark fantasy anime character portrait in shonen manga style with heavy ink outlines and warm forge glow lighting. A [male/female] dwarf is shown from the chest up, with short and stocky proportions, broad shoulders, and dense compact musculature. They have [HAIR COLOR] hair and [EYE COLOR] determined eyes. Their beard is elaborately braided and decorated with small metal ornaments. They wear heavy armor engraved with geometric runes, in a metallic palette of steel blue, bronze, and copper. The background glows with the warm amber light of a distant forge, with ember particles floating in the air. Their expression is proud and stubborn. [WEAPON OR TOOL DESCRIPTION].

### Halfling

> A dark fantasy anime character portrait in shonen manga style with soft ink outlines and warm firelight. A [male/female] halfling is shown from the chest up, with small stature, round soft facial features, and curly [HAIR COLOR] hair. Their [EYE COLOR] eyes are large, bright, and sharp with clever intelligence. They wear warm-toned patched traveling clothes in browns and creams, practical but well-loved. Their large bare feet are visible at the bottom of the frame. The background is a cozy firelit interior with deep shadows beyond. Their expression is a mischievous knowing smile. [ACCESSORY DESCRIPTION].

---

### Therian — Feline

> A dark fantasy anime character portrait in shonen manga style with fluid ink outlines and cool moonlit lighting. A [male/female] feline therian is shown from the chest up. They have large expressive eyes with vertical slit pupils in [EYE COLOR, preferably golden or amber], and prominent feline ears on top of their head that are alert and slightly angled. A single long furred tail is visible behind them. Their build is lithe and athletic with a graceful feline posture, and [FUR PATTERN] fur accents are visible on their cheeks and forearms. The color palette is warm — fawn, gold, and tawny tones against deep black shadows. The background is dark and atmospheric with silver moonlight. Their expression is confident and predatory. [CLOTHING OR ARMOR DESCRIPTION].

### Therian — Canine

> A dark fantasy anime character portrait in shonen manga style with strong ink outlines and dramatic side lighting cutting through a dark forest. A [male/female] canine therian is shown from the chest up. They have pointed wolf-like ears on top of their head and a bushy wolf tail visible behind them. Sharp fangs are slightly visible. Their [EYE COLOR] eyes are intense and loyal, and [FUR COLOR] fur accents mark their jawline and neck. Their build is athletic and muscular, radiating pack-protector energy. The color palette is grey and brown against deep shadows. Their expression is fierce and protective. [CLOTHING OR ARMOR DESCRIPTION].

### Therian — Vulpin

> A dark fantasy anime character portrait in shonen manga style with refined ink outlines and an ethereal mystical glow. A [male/female] vulpin is shown from the chest up — the most human-like of the therian, with delicate refined facial features. They have elegant fox ears on top of their head and a large, fluffy, voluminous fox tail that dominates the composition. Their eyes are a striking golden amber with an enigmatic depth. Their [HAIR COLOR, preferably red-orange or pure white] hair flows elegantly. The background is dark with faint floating spirit flames in blue-white foxfire. The color palette is red-orange and white against deep blacks. Their expression is knowing and enigmatic, as though they see more than they reveal. [CLOTHING DESCRIPTION — flowing, elegant].

### Therian — Raptor

> A dark fantasy anime character portrait in shonen manga style with sharp ink outlines and dramatic uplighting against a dark sky. A [male/female] raptor therian is shown from the chest up. Their hair transitions into natural plumage, and feather accents line their arms and neck. Their hands end in sharp talon-like claws. Their [EYE COLOR] eyes are sharp, piercing, and hawk-like, with a vigilant intensity. Their build is lean and aerodynamic. The color palette draws from [eagle: brown and gold / owl: grey and white / hawk: rust and cream]. Wind currents are visible in the background. Their expression is alert and watchful, scanning for threats. [CLOTHING DESCRIPTION — light and functional].

### Therian — Ursid

> A dark fantasy anime character portrait in shonen manga style with heavy ink outlines and warm firelight illumination. A [male/female] ursid therian is shown from the chest up — the most imposing of all therian. They have round bear ears and a massive frame with broad shoulders, thick limbs, and dense fur accents on their forearms and shoulders. Their [FUR COLOR, preferably dark brown or black] fur contrasts with [EYE COLOR] eyes that are surprisingly gentle and deep, creating a striking contrast with their intimidating size. The color palette is brown and black against warm amber firelight. The background is a dark cave or deep forest interior. Their expression is calm and stoic, with hidden kindness. [HEAVY ARMOR OR FUR CLOTHING DESCRIPTION].

### Therian — Reptilian

> A dark fantasy anime character portrait in shonen manga style with precise ink outlines and harsh sunlight casting deep shadows. A [male/female] reptilian therian is shown from the chest up. Visible scales cover their cheeks, neck, and arms in [SCALE COLOR: green, deep blue, or sand] tones. Their eyes have vertical slit pupils in [EYE COLOR: amber, gold, or red] with a cold, calculating gaze. Their facial structure is subtly alien and inhuman compared to other therian. A powerful muscular tail is partially visible. Their build is lean and powerful. The color palette is green and dark teal against harsh light and deep shadow. The background is a dark swamp or sun-baked desert. Their expression is unreadable and calculating. [CLOTHING DESCRIPTION — minimal or functional].

### Therian — Lagomorph

> A dark fantasy anime character portrait in shonen manga style with delicate ink outlines and dramatic contrast lighting. A [male/female] lagomorph therian is shown from the chest up. Their most prominent feature is very long, expressive rabbit ears that convey emotion through their position and angle. They have a small fluffy round tail. Their [FUR COLOR: white, cream, or soft grey] fur accents frame soft facial features, but their [EYE COLOR: pink, red, or brown] eyes are large, bright, and cautious — deceptively innocent in appearance but clearly alert to danger. Their build is agile and slender. The color palette is soft whites and creams against dark, threatening shadows, emphasizing the contrast between their gentle appearance and the harsh world. The background is a dark meadow or underground burrow. [LIGHT ARMOR OR TRAVELING GEAR DESCRIPTION].

---

### Natural Peoples — Flower-Woman

> A dark fantasy anime character portrait in shonen manga style with organic ink outlines and an ethereal bioluminescent glow. A flower-woman is shown from the chest up. Floral elements grow organically from her body — petals emerge from her hair and shoulders, and plant-like patterns are woven into her skin rather than worn as clothing. The design is built around [FLOWER TYPE: rose, lily, wisteria, etc.], with bioluminescent markings casting a faint glow. The color palette combines deep forest greens with vivid [FLOWER COLOR] accents against a very dark forest background. Her expression is serene and otherworldly, as though she belongs to the forest itself.

### Natural Peoples — Dryad

> A dark fantasy anime character portrait in shonen manga style with textured ink outlines and golden sunlight filtering through an ancient canopy. A [male/female] dryad is shown from the chest up. Bark texture blends seamlessly into their skin, and living branches and small leaves grow naturally from their body and hair. Wooden horn-like or antler-like growths crown their head. Moss accents soften the transitions between wood and flesh. Their eyes have a distinctive bark-ring pattern in the iris. The color palette is deep green and dark brown with golden sap highlights. The background is a dark ancient forest with massive trees. Their expression conveys ancient wisdom and patience.

### Natural Peoples — Earth Elemental

> A dark fantasy anime character portrait in shonen manga style with heavy textured ink outlines and a warm inner glow illuminating the scene. An earth elemental is shown from the chest up, with a golem-like humanoid form. Stone and crystal formations are integrated into their body, and cracks in their earth-textured skin reveal a warm amber glow beneath. Their eyes are like embedded gemstones, glowing with inner light. Geological layers and mineral veins are visible across their massive, heavy frame. The color palette is stone grey and dark earth with amber crystal accents. The background is a dark cavern with crystal formations catching the elemental's inner light. Their expression is stoic and immovable.

---

### Visitors — Modifier

Visitors use the exact same prompt as their host Kin body. Append this sentence at the end:

> There is a subtle otherworldly gleam in their eyes, and their body language carries a faint sense of displacement, as though the body is not entirely natural to them — small anachronistic micro-gestures hint at a soul from another world.

*The Visitor's difference is intentionally subtle. It's a feeling, not a costume. Don't over-describe it.*

---

## 3. Lighting Modules

Swap these phrases into any prompt to change the lighting. Replace the lighting sentence in your base prompt with one of these.

### Torchlight / Firelight

> The scene is lit by warm torch fire, casting a dancing orange glow across the subject's features. Shadows shift and flicker on their face, with ember particles floating in the air. Beyond the firelight, everything fades to deep black.

### Moonlight

> Cold silver moonlight falls from above, creating blue-white rim lighting along the subject's edges and deep blue shadows across their features. Stars are faintly visible in the dark sky behind them.

### Forest Canopy

> Dappled sunlight filters through a dense canopy of leaves, casting irregular patterns of warm light and cool shadow across the scene. The ambient light has a green tint, and fine dust particles are visible in the light beams.

### Overcast / Grim

> The light is flat and diffused under a heavy overcast sky, with no direct sunlight. Colors are muted and slightly desaturated. Fog or mist softens the edges of distant elements, creating a heavy oppressive atmosphere.

### Golden Hour

> Warm golden sunset light bathes the scene from a low angle, casting long dramatic shadows and painting everything in amber and orange tones. A warm rim light catches the edges of the subject's silhouette. Dust motes glow in the light beams.

### Storm / Dramatic

> The scene is lit by intermittent lightning against dark thunderclouds, creating harsh momentary contrast. Rain streaks across the frame and wet surfaces reflect the flash. Dramatic backlighting silhouettes the subject against the storm.

### Underground / Dungeon

> A single faint light source — a torch or a glowing crystal — provides the only illumination in an oppressive underground space. The light barely reaches beyond the subject, creating extreme contrast between the lit features and the consuming darkness around them.

### Magical Glow

> The scene is illuminated by [COLOR] magical energy radiating from [source: a spell, a weapon, a rune on the wall]. The supernatural light casts colored reflections on the subject's face and nearby surfaces, with faint arcane particles drifting through the air.

---

## 4. Environment Pre-Prompts

Full prompts for location illustrations without characters.

---

### Dense Forest

> A dark fantasy anime landscape illustration with detailed ink linework and atmospheric perspective. A dense primeval forest fills the frame, with massive ancient trees whose gnarled roots grip the earth. The canopy above is so thick that sunlight only enters as narrow god rays, illuminating patches of lush ferns, moss, and wildflowers on the forest floor. Fallen logs are slowly being reclaimed by fungus and vegetation. A fine mist hangs between the trunks, and the air feels heavy and alive. The deeper you look into the forest, the darker it becomes. A barely visible path winds between the trees. The palette is rich deep greens and dark browns with golden light accents. No people are visible.

### Dungeon / Ruins Interior

> A dark fantasy anime landscape illustration with heavy ink outlines on foreground elements and deep atmospheric shadows. The interior of ancient dungeon ruins stretches before the viewer — massive crumbling stone architecture with collapsed pillars and archways slowly being consumed by creeping vines and moss. A single torch mounted on a wall provides the only light, casting dancing shadows and revealing ancient carved runes that glow faintly on the walls. Water drips from the ceiling into puddles that reflect the warm light. Dust particles float in the single beam of illumination. The palette is dominated by deep stone grey and warm amber, with the darkness beyond the torchlight feeling absolute and oppressive. No people are visible.

### City / Town Street

> A dark fantasy anime landscape illustration with detailed ink linework and warm evening atmosphere. A narrow cobblestone street winds between multi-story timber and stone buildings in a medieval fantasy town. Hanging shop signs creak in a light breeze, and laundry lines stretch between buildings above. Market stalls with colorful awnings line one side of the street. Warm golden light spills from windows and open doorways, reflecting off wet cobblestones. The sky above shows the last amber glow of sunset against deepening blue. Every building tells a story through its wear, its repairs, its personality. The palette balances warm amber interior light against cool blue-grey evening shadows. No people are visible.

### Elven Settlement

> A dark fantasy anime landscape illustration with elegant ink linework and ethereal moonlit atmosphere. An elven city grows organically from massive ancient trees — living wood architecture spirals upward with bridges and walkways connecting platforms high in the canopy. Bioluminescent flowers and trailing vines provide a soft natural glow. The structures follow elegant organic curves, decorated with silver and violet filigree. Moonlight filters through the leaves, creating shifting patterns on reflective pools below. The air is filled with a fine ethereal mist. The palette is silver-green and deep purple against the dark forest backdrop. No people are visible.

### Dwarven Halls

> A dark fantasy anime landscape illustration with monumental composition and warm forge-glow atmosphere. A colossal underground dwarven hall stretches into darkness above, supported by massive carved stone pillars covered in intricate geometric runes. In the distance, the warm orange glow of active forges illuminates rivers of molten metal flowing through carved channels. Metallic veins in the stone walls catch and reflect the forge light in bronze and copper tones. The scale is overwhelming — every surface is carved, every pillar tells a story in stone. The palette is blue-steel and dark iron against warm forge orange and amber. No people are visible.

### Open Plains / Panorama

> A dark fantasy anime landscape illustration with sweeping panoramic composition and dramatic sky. Vast rolling grasslands stretch to the horizon, where a distant mountain range rises as dark silhouettes against a dramatic sky of towering clouds lit from below by a setting sun. An ancient stone road, cracked and overgrown, cuts through the middle ground, with a weathered monolith standing alone beside it for scale. Wildflowers and wind-blown grass fill the foreground. Atmospheric haze softens the distant features into blue-grey layers. The palette is amber and gold in the sky against deep blues and greens in the land. The sense of vast, beautiful emptiness is palpable. No people are visible.

### Swamp / Marshland

> A dark fantasy anime landscape illustration with eerie atmosphere and bioluminescent accent lighting. A dark fantasy swamp stretches before the viewer — gnarled dead trees rise from murky still water, their bare branches draped with hanging moss. Thick fog hangs low over the water surface. The only color comes from bioluminescent fungi and strange glowing plants scattered across rotting logs and muddy banks, casting an eerie green and purple glow. Tangled roots break the water surface, and bubbles occasionally rise from the dark depths. The palette is sickly green and grey-purple with oppressive humidity visible in the air. The sense of hidden danger beneath the water surface is pervasive. No people are visible.

### Battlefield Aftermath

> A dark fantasy anime landscape illustration with somber overcast atmosphere and muted color palette. An abandoned battlefield stretches across the frame — scorched and scarred earth, broken weapons and shattered shields embedded in the ground, tattered heraldic banners still standing on tilted poles. Craters and shallow trenches scar the landscape. The sky is heavy grey overcast. Crows and ravens circle above in the distance. Nature has begun to reclaim the field — grass pushes through ash, and small wildflowers grow around a discarded helmet. Morning mist softens the edges of everything. The palette is muted earth tones with occasional faded color from rusted metal and old fabric. No people, no bodies — only the aftermath. No people are visible.

### Ancient Portal Site

> A dark fantasy anime landscape illustration with mystical atmosphere and dual-toned magical lighting. Ancient portal ruins dominate the scene — a massive stone archway covered in carved runes that glow faintly with purple and teal light. Centuries of vegetation have overgrown the structure, with vines and roots wrapping around the carved pillars. Between the pillars, a faint shimmering energy distorts the air like heat haze. A circular stone platform at the base is carved with concentric symbols, partially buried under moss and fallen leaves. The surrounding area feels subtly warped by residual magic — trees grow at odd angles, and the light bends strangely. The palette contrasts purple-teal magical glow against dark stone and deep green vegetation. The sense of immense age and dormant power is overwhelming. No people are visible.

---

## 5. Composition Modifiers

Append these phrases to any prompt to control framing.

### Character Framing

- **Close-up portrait:** "Framed as a close-up of the face and shoulders, with the background softly blurred behind them."
- **Upper body:** "Shown from the chest up, with hands and arms partially visible and the environment providing context behind them."
- **Full body:** "Shown in full body, standing, with feet visible and the environment filling the frame around them."
- **Dynamic action:** "Captured mid-action in a dynamic pose, with a dramatic angle and a sense of explosive movement."
- **Low angle hero shot:** "Viewed from a low angle looking up, framed heroically against the sky, giving a sense of power and presence."

### Environment Framing

- **Establishing shot:** "A wide establishing shot showing the full environment at epic scale, with tiny details suggesting life and history."
- **Path perspective:** "A path leads the eye from the foreground deep into the distance, creating strong depth through vanishing-point composition."
- **Vertical scale:** "Composed vertically, looking up at a towering structure that fills the frame and emphasizes vertiginous scale."
- **Interior wide:** "A wide interior shot framed by an archway or doorway in the foreground, drawing the eye into the space beyond."

---

## 6. Quick Reference — Kin Color Palettes

Use these color descriptions to maintain visual consistency.

| Kin | Primary Palette | Accent Colors |
|-----|----------------|---------------|
| Human Civilized | amber, gold, warm red | cream, bronze, burgundy |
| Human Barbarian | steel blue, grey, white | ice blue, dark brown, blood red |
| Human Primitive | forest green, ochre, brown | bone white, rust, deep red |
| Elf | silver, violet, deep purple | moonlight blue, leaf green |
| Dwarf | steel blue, bronze, copper | forge orange, dark iron, gold |
| Halfling | warm brown, cream, forest green | sunset orange, berry red |
| Therian Feline | fawn, gold, tawny | amber eyes, dark rosettes |
| Therian Canine | grey, brown, dark slate | amber, russet, black |
| Therian Vulpin | red-orange, white, gold | foxfire blue, amber |
| Therian Raptor | brown-gold or grey-white | sharp yellow eyes, rust |
| Therian Ursid | dark brown, black, chestnut | honey amber, warm grey |
| Therian Reptilian | green, teal, sand | gold-amber eyes, dark jade |
| Therian Lagomorph | white, cream, soft grey | pink, pale rose, brown |
| Flower-Woman | green + flower-specific color | bioluminescent accents |
| Dryad | deep green, bark brown | moss, golden sap, amber |
| Earth Elemental | stone grey, dark earth | crystal amber, lava orange |

---

## 7. Anti-Patterns — What NOT to Write

Because Flux understands natural language, bad habits from SDXL prompting will actively hurt your results.

| Don't Do This | Do This Instead |
|---|---|
| `anime, dark fantasy, shonen, detailed, masterpiece, best quality` | "A dark fantasy anime illustration in shonen manga style with detailed ink linework" |
| `(expressive eyes:1.3), (long ears:1.2)` | "with particular emphasis on their large expressive eyes and prominently long pointed ears" |
| `1girl, elf, silver hair, purple eyes, forest` | "An elven woman with flowing silver hair and luminous purple eyes, standing in a dark ancient forest" |
| Negative prompt: `ugly, deformed, bad hands` | Simply don't mention it. Describe what you want, not what you don't. |
| `white background, simple background` | Describe the actual background you want: "against a dark atmospheric background with faint fog" |
| Repeating the same concept in different words for emphasis | State it once, clearly, and move on |

---

*Version 1.0 — March 2026*
*Designed for Flux 2 Klein 9B with Qwen3 8B text encoder on ComfyUI*
