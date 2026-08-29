# The Nichols Law Group — Design System

A reusable brand and interface system for **The Nichols Law Group**, a personal injury and criminal defense firm in Houston, Texas. It covers the main website and future paid landing pages, in English and Spanish.

## Who this is for

The visitor is not browsing. They are on a phone, minutes or hours after a car wreck, an arrest, or an injury, comparing three or four firms in the same few minutes. Every screen in this system is built as **decision support**, not as a brochure: the phone number is always visible, the primary action is always one thumb-reach away, and the proof the firm can actually substantiate (4.9★ from 91 Google reviews, phones answered 24/7, nothing owed unless they win) is presented at the scale of a headline rather than as a footnote.

The firm's positioning is *established and winning* — confident, serious, warm where it is genuinely warm (a named medical coordinator on staff; a family-forward attorney), never cute, never startup-y, and never the templated PI look.

## Sources given

- `uploads/Nichols-Law-Group-Image-Assets (1)/` — 30 de-duplicated images extracted by DSG from 29 saved pages of the current site (5 zipped page saves + 24 self-contained HTML saves), plus `IMAGE-INSTRUCTIONS.md`, the handoff note describing each file's intended use. Everything usable was copied into `assets/`.
- The written brief (brand constraint, audience, personality, colour and type direction, bilingual requirement, component inventory, things to avoid).
- **The live site, `lesternicholslaw.com`** — read on 25 Aug 2026 for the firm's real contact details, page structure, practice-area IA, footer, disclaimer and homepage copy. Everything in this system that states a fact about the firm now comes from there (see "Facts of record" below).
- **No codebase, Figma file, style guide, font binaries, or slide template were provided.** No live-site CSS was available, so the token values here are authored from the brief plus colours sampled directly out of the logo PNG — they are not extracted from an existing stylesheet. (The logo file on the live site is named `Nichols_Logo-Astronaut-Blue`, which is consistent with the `#27396c` sampled from the artwork.)

### Sampled from the artwork

| Value | Source |
|---|---|
| `#27396c` | monogram fill, `logo-primary-horizontal.png` (dominant non-transparent colour) |
| `#231f20` | wordmark black, same file |

### Facts of record

Taken from `lesternicholslaw.com` — these are the only firm facts this system asserts. Change them here first if the firm changes them.

| | |
|---|---|
| Legal name | The Nichols Law Group, PLLC |
| Trading site | lesternicholslaw.com ("Lester Nichols Law") |
| Attorney | Lester B. Nichols III, Esq. — Managing Partner & Attorney |
| Staff | Christian Bautista — Medical Coordinator |
| Primary phone | (713) 705-2250 |
| Toll-free | (844) NLG-WINS · (844) 654-9467 |
| Email | law@lesternichols.com |
| Office | 9408 Cypress Creek Parkway, Houston, Texas 77070 |
| Hours | Open 24 hours |
| Rating | 4.9★ from 91 Google reviews |
| Tagline | "Life Moves Fast and Accidents Happen" |
| Practice IA | Auto Accidents (7) · Personal Injury (6) · Criminal Defense · Diminished Value Claims = 15 |
| Nav | Home · About Us · Practice Areas · Contact Us |

**No verdict or settlement figures.** The live site publishes none — it says only "multiple high dollar settlements". Every dollar figure that previously appeared in this system was illustrative and has been removed. `CaseResultCard` stays in the kit; until Lester supplies verified numbers with the matching *past results* footnote, use it for rating, review-count and availability figures instead.

> **Note (per the Master Build Spec, `docs/app/03-DESIGN.md` and the top-level build spec doc):** Criminal Defense is cut from the rebuilt site's scope. Where this design system references Criminal Defense (imagery, practice IA, content), treat it as inherited context from the original brief, not as current build scope — defer to the Master Build Spec's locked decisions.

## Brand constraints to respect

1. **The navy is the brand.** `--navy-600: #27396c` came out of the existing logo. Do not shift it.
2. **There is no reversed/white logo file.** Nothing in either capture batch contains one. So: headers and any surface carrying the logo image stay light (paper or white), and on navy the firm name is set **typographically** (`<Wordmark tone="light" />`) — see the "On navy: type, not logo" card. Never drop the navy PNG into a white chip on a dark field. If the client produces a white logo, that rule can be relaxed.
3. **Accent is gold, not red.** Navy + red on a PI site reads as either political or alarmist; burnished gold (`--gold-600 #a97a15`) reads as established and pairs with navy without competing with it. Status red exists (`--red-600`) but is reserved for form errors and is never a CTA.
4. **Imagery is stock and should be treated as such.** All 20 practice-area photos are generic licensed stock. They are desaturated ~28% and sit under a navy bottom gradient so they read as brand texture rather than as stock photography. Custom photography is the single highest-value upgrade available to this brand.
5. **No gavels, columns, or handshakes as primary imagery.** The one gavel/scales stock shot is quarantined for policy pages. The monogram already carries the column-and-scales idea; repeating it in photography is what makes competitor sites look interchangeable.
6. **Lester's professional bio is still outstanding** (the current site says "Bio Coming Soon", while the kids' bios are fully written). Placeholder copy in this system stays factual — do not invent credentials, awards, or bar admissions.

---

## CONTENT FUNDAMENTALS

**Voice: plain-spoken authority.** Short declarative sentences. No throat-clearing, no legalese in marketing copy, no exclamation marks.

- **Person.** Speak to the reader as **you**; speak for the firm as **we**. Never "the firm" or "our team of dedicated professionals". Lester is "Lester Nichols" on first mention, "Lester" in warm contexts (the family section), "Mr. Nichols" nowhere.
- **Sentence length.** Headlines 3–8 words. Body sentences under 20 words. An anxious person skimming on a phone reads about two lines before deciding.
- **Casing.** Sentence case for headlines and subheads. UPPERCASE only for eyebrows, button labels, and micro-labels (with tracking — `--tracking-eyebrow` / `--tracking-caps`). Never Title Case A Sentence Like This.
- **Numerals.** Always numerals, never words: "4.9★", "91 reviews", "24/7", "(713) 705-2250". Abbreviate large figures so they stay on one line on a phone. Phone numbers are always tappable and always shown as digits — never hidden behind "Contact us".
- **Claims.** Concrete and attributable, never superlative. Write "4.9★ from 91 Google reviews" not "aggressive representation you can trust". Never invent a verdict or settlement figure — the firm has published none. Anywhere a case figure does appear, the *past results do not guarantee a similar outcome* line appears in the same view.
- **Fee language.** "No fee unless we win" — plain, repeated, never in a fine-print voice.
- **Reassurance beats persuasion.** The most valuable sentence on the page is usually operational: "We answer the phone at 2am." "Christian tracks every doctor visit." "The consultation is free and takes ten minutes."
- **CTA labels.** Verb-first and specific, and matched to the live site's own words: *Get a FREE consultation*, *Complimentary consultation*, *Call (713) 705-2250*. Never *Submit*, *Learn more* (except as a card affordance), *Click here*.
- **No emoji, anywhere.** The only glyph used decoratively is ★ for ratings and → on card affordances.
- **Spanish is a mirror, not a footnote.** Every page has a full Spanish counterpart; the toggle says `ES` / `EN`, never a flag icon. Spanish copy is translated, not machine-echoed: "¿Lesionado en un accidente? Llámenos ya." Assume Spanish strings run ~20–25% longer than English.

Examples of the register:

> **Life moves fast and accidents happen.** We answer 24 hours a day. The consultation is free, and we don't get paid unless you do.
> **Insurance companies have attorneys.** You should have one too.
> **Christian Bautista, Medical Coordinator.** He tracks your treatment — ER, physical therapy, MRIs — so you don't have to chase records.

---

## VISUAL FOUNDATIONS

**The idea in one line:** a warm off-white document, set in an authoritative serif, with navy structure and one gold action colour — closer to a well-set legal brief than to a landing page.

> **Note:** the token files ship the display font-family as `Archivo` (a sans, not a serif) per `--font-display` in `tokens/typography.css`/`_ds_manifest.json` — this is the built value. The paragraph below (from the original brief/readme) called for a serif; treat the shipped `Archivo` sans as the locked, current decision per the CLAUDE.md design-preferences note ("No serif display face by default... favor an authoritative sans... e.g. Archivo") which supersedes the earlier serif direction. Flag any conflict to the user before changing fonts.

**Colour.** Navy (`--navy-600`) is structure and headings; deep navy (`--navy-800/900`) is the only dark field, used for the footer, one or two conviction bands, and the sticky bar. Warm off-white `--paper #faf8f4` is the page; white is reserved for cards so they lift off the page without a heavy shadow. Gold appears in exactly three roles: primary CTA fill, the 3px top rule on anything that converts, and eyebrow/star accents. Two background colours per page, maximum. No gradients as decoration — the only gradients in the system are photographic scrims (`--scrim-navy`, `--scrim-bottom`) and the soft radial behind transparent headshots.

**Type.** Display: **Archivo** (600/700/800) — see note above on the serif/sans supersession. Body/UI: **Source Sans 3** (400/600/700) at 17px / 1.6, capped at 64ch. Settlement figures use the display face with `lining-nums tabular-nums` at `--text-figure` (up to 7rem) — the figure is the largest thing on the screen by a wide margin. Eyebrows are 12px uppercase at `0.14em`.

**Layout.** 1200px container (760px for reading-width pages, 1400px for full-bleed bands), fluid gutters `clamp(20px, 5vw, 48px)`, fluid vertical section rhythm `clamp(56px, 7vw, 112px)`. Grids are `auto-fill minmax()` so the 15-area practice grid reflows from 1 to 4 columns with no media queries. Fixed elements: the sticky header (light, blurred, `backdrop-filter`) and the mobile sticky call bar (fixed bottom, 64px + safe-area inset). Pages reserve 84px of bottom padding so the bar never covers content. Never put a headline in a fixed-height box — Spanish will break it.

**Cards.** White, 1px `--border-hairline` (#e0dad2), **4px** radius, `--shadow-sm`. Anything that converts — case results, intake forms — adds a **3px gold top rule**. On navy, cards become `--navy-700` with a 16%-white border. Controls use a 2px radius; the only pill in the system is the EN/ES toggle. No coloured left-border cards, no glassmorphism, no double borders.

**Shadows.** Shallow and cool, tinted with the navy (`rgba(16,24,41,…)`): `xs` for tiles, `sm` for cards, `md` on card hover, `lg` for overlays, and one warm gold-tinted `--shadow-cta` under the primary button. The sticky bar casts upward (`--shadow-sticky`).

**Imagery.** Photography is cool-to-neutral, never warm-filtered, never black and white, no grain. Practice-area photos: `saturate(.72) contrast(1.04)` under a `rgba(16,24,41,.15) → .72` bottom gradient. The Houston skyline hero already ships with a navy overlay baked in and is used full-bleed behind the homepage hero at low contrast. Transparent-background people PNGs sit on a `--navy-50` radial panel, bottom-aligned, cropped from the top. The monogram appears as a watermark exactly once per page at ≈8% opacity, bleeding off an edge, never over text.

**Transparency and blur.** Used in two places only: the header's `rgba(250,248,244,.94)` + blur, and white-at-6–10% surfaces inside navy bands. No blurred cards, no frosted overlays on photos — protection for text over photos comes from a solid-direction gradient, not from blur.

**Motion.** Restrained: 120/180/320ms on `cubic-bezier(.2, .6, .25, 1)`. Fades, 3px nudges (the card →), and a 1.03 image scale on card hover. No bounces, no springs, no scroll-jacking, no counting-up animation on settlement figures — the number is authoritative, not a slot machine. `prefers-reduced-motion` is honoured globally in `tokens/base.css`.

**States.** Hover *darkens* fills (gold-600 → gold-500 reads as brighter/warmer; navy-600 → navy-700) and lifts cards from `xs` to `md` with a border shift to `--navy-300`. Press drops the control 1px — no scale-down. Focus is a 2px gold outline at 2px offset, everywhere, never removed. Disabled is 45% opacity with `not-allowed`. Links are navy, underlined at 1px / 2px offset, and go gold on hover.

**Borders and rules.** One hairline weight (1px `--ink-200`) for structure; 2px for the small gold eyebrow rule; 3px for the gold top rule on converting surfaces. Section dividers are hairlines or a change of background, never both.

---

## ICONOGRAPHY

**The source contains no icon set.** The 29 captured pages yielded only the previous page-builder's decorative shapes, social glyphs, and tracking pixels — all excluded from the handoff as non-content. There is therefore no brand icon font, sprite, or SVG library to copy in, and this system deliberately does not invent one.

The approach that follows from that:

- **Type and rules carry hierarchy, not icons.** Eyebrow + gold rule replaces the "icon in a circle above a heading" pattern that makes PI sites look templated. Practice-area cards are identified by photograph and name; case results by the figure itself.
- **Two Unicode glyphs are sanctioned**, both already used in the components: `★` for ratings (gold, `--star-color`) and `→` for the card "Learn more" affordance. A `▾` marks the select control. Nothing else.
- **No emoji, ever.**
- **If a project genuinely needs UI icons** (a phone glyph in the sticky bar, a chevron in an accordion), use **Lucide** from CDN at `stroke-width: 1.75`, sized 20/24px, coloured `currentColor`. This is a *flagged substitution*, not brand truth — Lucide's geometric line style is the closest neutral match to the logo's thin engraved linework. Prefer no icon over a decorative one.
- **The monogram is not an icon.** `assets/brand/logo-icon-mark.png` is the app icon / favicon and the watermark seed. It is never inlined next to text as a bullet or badge.

---

## Typography substitution (needs your input)

No font binaries came with the assets, and no live CSS was available to read the current site's stack from. **Source Serif 4** and **Source Sans 3** were the original brief's proposed substitution; the CLAUDE.md design-preferences note (below) explicitly rejects a default serif display face ("No serif display face by default... favor an authoritative sans... e.g. Archivo, not Fraunces/Playfair"), and the shipped tokens use **Archivo** for display instead — see the Visual Foundations note above. If the firm has licensed brand fonts — or if the current site uses something specific worth keeping — send the files and this swaps out in one file (`tokens/fonts.css`).

---

## Index

**Root**
- `styles.css` — the single entry point consumers link. `@import`s only.
- `readme.md` — this file. `SKILL.md` — portable skill wrapper.
- `thumbnail.html` — homepage tile.

**Tokens** (`tokens/`) — `fonts.css`, `colors.css`, `typography.css`, `spacing.css`, `radius.css`, `elevation.css`, `motion.css`, `base.css` (element resets).

**Foundations** (`guidelines/`) — 21 specimen cards, grouped in the Design System tab as **Colors** (navy, gold, ink & paper, status, approved pairings), **Type** (display, body, settlement figures, eyebrows, scale, bilingual test), **Spacing** (scale, section rhythm, tap targets), **Brand** (logo lockup, on-navy rule, watermark, imagery treatment, cards & radii, shadows, motion & states).

**Components** (`components/`) — each with `.jsx`, `.d.ts`, `.prompt.md`, and one card HTML per directory.

| Group | Components |
|---|---|
| `core/` | **Button**, **Wordmark**, **Eyebrow** |
| `trust/` | **CaseResultCard**, **TrustBadge**, **TestimonialCard** |
| `people/` | **StaffCard** |
| `practice/` | **PracticeAreaCard**, **PracticeAreaGrid** |
| `forms/` | **Field**, **Input**, **Select**, **Textarea**, **CaseIntakeForm** |
| `navigation/` | **SiteHeader**, **StickyCallBar**, **SiteFooter** |

**Intentional additions** (not named in the brief, added because the named components could not stand without them): **Button**, **Wordmark**, **Eyebrow** (shared primitives every other component composes), **Field / Input / Select / Textarea** (the intake form's parts, exposed so landing pages can build their own variants), **PracticeAreaGrid** (the responsive wrapper that makes the 15-area grid work on both hub and landing pages), **SiteHeader / SiteFooter** (needed for the UI kits to be real screens).

**UI kits** (`ui_kits/`)
- `website/` — the main site: homepage, practice-area hub, practice-area detail, about/team, contact. Click-through, with a working EN/ES toggle.
- `landing_page/` — a paid-traffic landing page (single conversion path, no site nav).

**Templates** (`templates/`)
- `landing-page/LandingPage.dc.html` — the paid landing page as a copyable starting point for consuming projects (loads this system via `ds-base.js`).

**Assets** (`assets/`) — `brand/` (3 logo files), `people/` (5), `imagery/` (2), `practice-area/` (20). All copied verbatim from the handoff; nothing was drawn or generated. Original assets live in Google Drive under "Nichols Law Group — DSG Project"; not all binaries are checked into this repo yet — pull individual files from Drive as pages are built (see `IMAGE-INSTRUCTIONS.md` for the full manifest and intended use of each).

---

## Component behavior contracts, guidelines cards, and full asset binaries

This readme, the design-preferences note (below), and `tokens/*.css` are the buildable core checked into this repo. The full component `.jsx`/`.prompt.md` source, the 21 guideline specimen cards, the two UI-kit screens, and the raw image binaries live in the source design-system export (Google Drive, "Nichols Law Group — DSG Project" → "Nichols Law Group Design System.zip", unzipped) and were not all individually copied into this repo on first pass — pull specific files from there as each page/component is implemented, rather than assuming everything is already local. `_ds_manifest.json` in this folder is the full machine-readable index (every token, every component, every card, every path) if you need to enumerate what exists before pulling a specific file.
