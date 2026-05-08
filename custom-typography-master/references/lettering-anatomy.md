# Lettering Anatomy Reference

The vocabulary that makes Nano Banana Pro produce drawn-feeling type instead of
system fonts. Use these terms precisely in prompts. The more specific, the better.

---

## Stroke Structure

**Stroke weight**
- `hairline stroke` — ultra-thin, ornamental, high contrast with main stroke
- `thin stroke` — secondary stroke, lighter than main but visible
- `medium stroke` — balanced weight across all strokes
- `heavy stroke` — dominant weight, minimal contrast
- `monoline stroke` — uniform weight throughout, no thick-thin variation

**Stroke contrast**
- `high stroke contrast` — dramatic thick-to-thin variation (calligraphic influence)
- `moderate stroke contrast` — some variation, readable as drawn
- `zero stroke contrast` / `monoline` — uniform weight, geometric or grotesque

**Stress axis** (direction the thickest strokes run)
- `vertical stress` — thickest part of curves at 12 and 6 o'clock positions
- `diagonal stress` — thickest part runs at approximately 45 degrees (old style)
- `oblique stress` — slightly off-vertical, feels more organic

---

## Serif Types

**Slab serifs**
- `flat bracket slab serif` — rectangular, unbracketed transition from stroke
- `bracketed slab serif` — smooth curved transition into serif foot
- `wedge slab serif` — triangular serif, wider at tip, narrows at attachment
- `Egyptian slab` — thick, heavy slab equal in weight to stroke
- `clarendon slab` — thick slab with slight bracket, Victorian heritage

**Traditional serifs**
- `fine hairline serif` — delicate line terminus, high contrast bodies
- `cupped serif` — slightly hollowed on top, traditional inscribed feel
- `bilateral serif` — extends equally both directions from stroke
- `unilateral serif` — extends only one direction
- `rounded serif` — slightly softened at terminus

**Script/Brush serifs**
- `pen-cut sheared terminal` — letterforms end at pen angle (calligraphic)
- `ball terminal` — perfectly round terminus
- `teardrop terminal` — pear-shaped terminal on curved strokes
- `swash terminal` — extended decorative stroke finish

**No serif (sans)**
- `sheared terminal` — cut at angle, humanist feel
- `rounded terminal` — small arc at stroke end, friendly
- `flat-cut terminal` — perpendicular to stroke direction, geometric
- `tapered terminal` — stroke narrows to a point

---

## Letterform Weight and Proportion

**Weight descriptors**
`ultralight` / `light` / `book` / `regular` / `medium` /
`semibold` / `bold` / `heavy` / `black` / `ultra black`

**Width descriptors**
`ultra condensed` — very narrow, tall letterforms
`condensed` — noticeably narrow
`semi-condensed` — slightly narrower than normal
`normal` / `regular` — standard proportion
`semi-extended` — slightly wider than normal
`extended` — noticeably wide
`ultra extended` — very wide letterforms

**Best combinations for badge work:**
- `ultra condensed heavy` — maximum typographic density, classic badge
- `condensed bold` — classic athletic, highly readable
- `extended medium` — commanding, authoritative
- `condensed ultra black` — maximum impact, tight badge

---

## Capital Letters and Case

`all caps` — traditional for badge/emblem headline
`small caps` — elegant, refined secondary text
`titling caps` — full-height capitals optimized for display size
`mixed case` — adds humanity, less formal
`initial cap + lowercase` — approachable, brand name feel

---

## Special Letterform Features

**Inline treatment**
`inline detail on main strokes` — hairline channel cut through thick strokes, creates
depth without dimensional rendering. Classic in heritage and Victorian display type.

**Outline treatment**
`double outline on letterforms` — inner + outer rule creating a layered effect
`single rule outline, even weight` — simple, clean secondary definition
`offset shadow outline` — rule shifted down-right, creates dimensional feel flat

**Dimensional treatments** (use carefully with Nano Banana)
`3D perspective extrusion on letterforms` — letters receding into space
`block shadow, letterforms with uniform right-and-down depth` — flat 3D look
`beveled letterforms` — edges cut at angle, engraved feeling

**Interior details**
`crossbars with decorative end caps` — horizontal strokes finished with small serifs
`spurred uppercase G` — spur on the C-opening of the G, traditional
`double-story lowercase a` — more typographic, less geometric
`single-story lowercase a` — geometric feel, humanist
`alternate letterforms` — swash alternate on K, R, Q — extended decorative legs

---

## Connections and Spacing

**Letterspacing**
`tight letterspacing` — letters nearly touching, dense and forceful
`normal letterspacing` — default optical spacing
`tracked out` — deliberate open spacing between letters
`zero spacing / touching letters` — letters share stroke space, very dense

**Ligatures**
`decorative ligature on CT, ST, TH` — joined letters sharing a crossbar
`contextual ligature in script` — natural pen connections between letters
`no ligatures` — clean, non-connected, geometric feel

**Baseline variation** (for hand-lettered feel)
`consistent baseline` — formal, typeset feeling
`slight bounce baseline` — organic, hand-drawn energy
`deliberate arched baseline` — type running in a curve (badge top/bottom arc)
`staggered baseline` — alternating up/down, extreme informal

---

## Script and Brush Lettering

**Script weights and feel**
`thin copperplate script` — formal, fine strokes, high contrast
`heavy brush script` — bold, high energy, thick-thin from brush pressure
`flat pen calligraphy` — optical consistent width change at 45 degrees
`pointed pen script` — high contrast, pressure-based stroke width

**Script connection style**
`connected script` — all letters joined in one flowing stroke
`semi-connected script` — some letters lift, natural variation
`disconnected script` — individual letterforms, script feel without flowing
`loop-and-return connections` — visible pen lift and reconnect marks

---

## Prompt Assembly Examples

**Bad (generic):**
`bold serif font in a badge`

**Good (surgical):**
`ultra condensed heavy slab serif with bracketed serifs and high stroke contrast,
flat terminals on the horizontal strokes, inline hairline detail running through
the main vertical stems, tight letterspacing with letters nearly touching`

**Bad:**
`handwritten script`

**Good:**
`heavy brush script with deliberate thick-thin pressure variation, ball terminals
on ascending strokes, slight bounce baseline, semi-connected with lifted strokes
between words only, pen angle approximately 30 degrees`

---

## Nano Banana Pro-Specific Notes

- **More anatomical description = better results.** The model responds to craft vocabulary.
- **Name the stress axis.** It changes the feel dramatically.
- **Inline detail is highly responsive.** Nano Banana renders inline strokes well.
- **Short text + detailed letterform = the sweet spot.** Long text dilutes quality.
- **Script prompts should mention pressure variation.** It's the signal for handmade feel.
- **Always pair letterform description with texture.** The texture grounds the type style.
