# custom-typography-master

A boutique-agency-level typography and lettering design skill for AI image generation. Built to produce badge, merch, apparel, and brand identity graphics at the level of Lincoln Design Co, Hoodzpah, and Doublenaut — using Nano Banana Pro and GPT Image 2 via Higgsfield.

---

## What This Is

Most AI image generation for typography produces generic outputs because prompts describe type in vague terms and the model has no visual target to aim at. This skill fixes both problems.

It combines:
- A structured prompt architecture that describes letterforms surgically
- 64 curated visual reference images across 11 style categories
- A reference routing system that matches any brief to the right images
- Style profiles for 20 named aesthetic systems

The result is prompts that tell the model exactly what to make — and reference images that show it.

---

## Repo Structure

```
custom-typography-master/
├── SKILL.md                          # Master skill — prompt architecture and rules
├── README.md                         # This file
├── references/
│   ├── style-systems.md              # 20 named style profiles with prompt vocabulary
│   ├── lettering-anatomy.md          # Surgical letterform description vocabulary
│   ├── badge-composition.md          # Badge, emblem, and lockup spatial systems
│   ├── texture-vocabulary.md         # Texture, treatment, and finish language
│   ├── color-systems.md              # Named palette systems by era and aesthetic
│   └── studio-references.md          # Lincoln Design Co, Hoodzpah, Doublenaut, etc.
└── visual-references/
    ├── README.md                     # Full image catalog — what each image teaches
    ├── badge-compositions/           # 9 badge shape and hierarchy references
    ├── heritage-americana/           # 8 original source material images
    ├── heritage-workwear/            # 2 direct workwear DNA references
    ├── letterform-references/        # 3 type specimen references
    ├── monogram-marks/               # 4 interlocked letterform constructions
    ├── moto-iron/                    # 12 moto, trade, fire, and speed references
    ├── script-lettering/             # 9 script style references
    ├── shape-systems/                # 2 badge shape anatomy references
    ├── slab-serif-display/           # 4 slab weight and width references
    ├── vintage-athletic/             # 8 sports patch and pennant references
    └── western-ranch/                # 3 western brand system references
```

---

## How To Use It

### 1. Read the SKILL.md

The skill routes every job through a 6-step process:

1. Classify the output type (badge, apparel graphic, wordmark, patch, etc.)
2. Load the matching style profile from `references/style-systems.md`
3. Load composition rules from `references/badge-composition.md`
4. Load letterform vocabulary from `references/lettering-anatomy.md`
5. Build the prompt using the 9-element architecture
6. Output a production-ready prompt with aspect ratio and model recommendation

### 2. Select Reference Images

Every prompt should be paired with 3-5 reference images from `visual-references/`. The `visual-references/README.md` catalogs every image with:
- What it teaches
- Which style profiles it covers
- Whether it's STRONG (send to model as reference input) or PARTIAL (vocabulary only)

### 3. Pass References to the Model

Using Higgsfield CLI:

```bash
# Upload reference images
higgsfield media upload --file visual-references/heritage-workwear/hillbilly-flannel-rocker-workwear.jpg
higgsfield media upload --file visual-references/heritage-americana/carhartt-vintage-ad-workwear.jpg

# Generate with references
higgsfield generate image \
  --model gpt_image_2 \
  --quality high \
  --resolution 2k \
  --aspect-ratio 4:3 \
  --ref MEDIA_ID_1 \
  --ref MEDIA_ID_2 \
  --prompt "your prompt here"
```

Raw image URLs for reference uploads (public repo):
```
https://raw.githubusercontent.com/woodfireddesigns/custom-typography-master/master/visual-references/[category]/[filename]
```

---

## The 9-Element Prompt Architecture

Every prompt must contain all 9 elements in order:

| # | Element | Purpose |
|---|---|---|
| 1 | Design type declaration | Tells the model what kind of object it's making |
| 2 | Exact text in quotes | Always explicit, always quoted |
| 3 | Letterform description | Surgical anatomy — not "bold serif", full description |
| 4 | Compositional system | Spatial logic of the layout |
| 5 | Texture and surface treatment | What makes it feel handmade |
| 6 | Color system | Specific palette language, not "vintage colors" |
| 7 | Style anchor | Era, studio, or aesthetic reference |
| 8 | Rendering instructions | Flat vector, apparel print, white background, etc. |
| 9 | Quality flags | Boutique studio quality, no amateur clip art |

---

## Style Profiles Covered

| # | Style | Key References |
|---|---|---|
| 1 | Heritage Americana | Carhartt, Filson, WPA, railroad badges |
| 2 | Vintage Athletic | Pennants, chenille patches, varsity jackets |
| 3 | Pacific NW Outdoor | Howler Brothers, Yeti, Patagonia |
| 4 | Action Sports / Skate | Lincoln Design Co, DC Shoes |
| 5 | Craft Beverage / Brewery | Founders, Dogfish Head, craft labels |
| 6 | Moto / Iron & Speed | Harley, Biltwell, board track racing |
| 7 | Western / Ranch / Rodeo | Pendleton, Tecovas, rodeo programs |
| 8 | Military / Tactical | WWII stencil, unit patches, AMA racing |
| 9 | Surf / Coastal | Hang Ten, Endless Summer, vintage contest |
| 10 | Premium Streetwear | Supreme, Off-White, Palace |
| 11 | Hunting / Fishing | Orvis, Filson, duck stamp |
| 12 | Concert Poster | Hatch Show Print, Third Man Records |
| 13 | Boxing / Fight Sports | Madison Square Garden, Everlast |
| 14 | Golf / Country Club | Augusta, R&A, classic crests |
| 15 | Psychedelic / Retro | Victor Moscoso, AOR rock |
| 16 | Streetwear Grunge | Stussy, Wu-Tang, 1990s NYC |
| 17 | Food / Farm to Table | Jacobsen Salt, Blue Bottle, artisan labels |
| 18 | Hard Rock / Metal | Iron Maiden, AC/DC era |
| 19 | Tech / Modern Geometric | Bauhaus, Swiss grid, IBM Plex |
| 20 | Dark Americana / Gothic | Jack Daniel's, tattoo flash, southern gothic |

---

## Key Rules — Never Break

1. **Always describe letterforms explicitly.** Anatomical description produces drawn-looking type. Generic names produce generic results.

2. **Name the texture.** One specific texture descriptor changes everything. Untextured prompts produce flat digital outputs.

3. **Short text strings.** 1-4 words per element. Complex multi-line layouts need each line described separately.

4. **Anchor to an era or studio.** Aesthetic references activate entire visual systems in the model's training.

5. **Declare the surface.** Apparel, packaging, woven patch — the output renders completely differently based on declared surface context.

6. **Flat vector beats photo-real for type.** Always specify `flat vector graphic` for badge and merch work.

7. **Quality flag at the end, every time.** Removes ambient AI aesthetic drift.

8. **Reference images are the unlock.** Text prompts alone will always drift toward the generic. Reference images show the model the actual target. Never generate without them.

9. **Composition before decoration.** The type hierarchy and spatial logic must be correct first. Texture, color, and ornament are secondary. A well-composed two-color badge beats an over-decorated four-color mess every time.

10. **Never arc a short brand name.** Perimeter arc type only works for brand names of 15+ characters. Shorter names stretch, lose weight, and lose legibility. Use horizontal, stacked, or rocker compositions instead.

---

## Model Recommendations

| Job | Model | Settings |
|---|---|---|
| Hero badges, packaging, client deliverables | Nano Banana Pro | 2K, high quality |
| Iteration, exploration, speed rounds | Nano Banana 2 / GPT Image 2 | 1K or 2K |
| Complex multi-element compositions | GPT Image 2 | high quality, 2K |
| Apparel full back graphics | GPT Image 2 | high quality, 2K, 2:3 ratio |

---

## Adding to the Library

When adding new visual references:

1. Place images in the correct category folder under `visual-references/`
2. Use descriptive filenames: `brand-style-descriptor.jpg`
3. Add a catalog entry to `visual-references/README.md` with:
   - What it shows
   - What it teaches
   - Style profiles it covers
   - Prompt vocabulary it activates
   - Reference strength (STRONG or PARTIAL)

Categories not yet fully covered: Concert Poster, Action Sports, Craft Beverage (non-western). Add as jobs require them.

---

## Built By

Wood Fired Designs — Michael Deschenes
`woodfireddesigns.com`

Built with Claude, iterated on real client jobs.
