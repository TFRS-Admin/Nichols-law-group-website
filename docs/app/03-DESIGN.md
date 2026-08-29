# Design

## Approved design inputs
**Design package:** `docs/app/design-system/` — "The Nichols Law Group — Design System" (DSG handoff, imported 2026-08-29 from the client-supplied Drive zip export).
**Approved build brief/design:** the top-level Master Build Spec doc (`NicholsBuildSpecMaster.md`, provided for the prototype build) governs copy, page scope, and locked project decisions. Where the two conflict, see Conflicts below.

## Implementation rule
The approved design is a specification, not necessarily production code. Preserve its visual language, hierarchy, states, responsive behavior, components, content intent, and interaction patterns while implementing appropriately in Base44.

Do not redesign approved UX because another pattern is preferred.

## Design-system usage
- **Start here:** `docs/app/design-system/readme.md` — full design rationale, brand constraints, content voice rules, visual foundations (color/type/layout/motion), and an index of every folder in the source export.
- **Design preferences (always apply):** `docs/app/design-system/design-preferences.md` — sitewide "never do this / favor this" rules locked in from prior review rounds; check new components against this before presenting.
- **Canonical tokens (checked into this repo, ready to consume):** `docs/app/design-system/tokens/*.css` — `fonts.css`, `colors.css`, `typography.css`, `spacing.css`, `radius.css`, `elevation.css`, `motion.css`, `base.css` (element resets). These are the literal token values; import in that order (fonts → colors → typography → spacing → radius → elevation → motion → base), matching `_ds_manifest.json`'s `globalCssPaths`.
- **Machine-readable index:** `docs/app/design-system/_ds_manifest.json` — every token, component, guideline card, and UI-kit path in the source export, with the token values inlined.
- **Image assets:** `docs/app/design-system/IMAGE-INSTRUCTIONS.md` — manifest of all 30 image assets and intended use per page. Raw binaries are **not** checked into this repo (they're large); pull individual files from the source Google Drive folder ("Nichols Law Group — DSG Project") as each page is implemented.
- **Not yet copied into this repo:** the full component `.jsx`/`.d.ts`/`.prompt.md` source (Button, Wordmark, Eyebrow, CaseIntakeForm, Field/Input/Select/Textarea, SiteHeader/StickyCallBar/SiteFooter, StaffCard, PracticeAreaCard/Grid, CaseResultCard/TrustBadge/TestimonialCard), the 21 guideline specimen HTML cards, and the two UI-kit reference screens (`ui_kits/website/`, `ui_kits/landing_page/`). These live in the source Drive export — pull the specific file(s) needed for the component/page currently being built rather than assuming they're already local. `_ds_manifest.json` lists every path.

## Project-specific UX rules
- **Font conflict, resolved in favor of the shipped tokens:** the design system's prose readme calls for a serif display face; the tokens actually ship `--font-display: "Archivo"` (a sans), consistent with the `design-preferences.md` rule "No serif display face by default... favor an authoritative sans... e.g. Archivo". Build against the shipped `Archivo` token value, not the serif described in prose. Flag to the user before changing this.
- **Criminal Defense is cut from build scope** (per the Master Build Spec, locked 2026-08-28) even though the design system's source imagery/content inherits language from an earlier brief that included it (e.g. `criminal-defense.jpg` in the image handoff). Do not build a Criminal Defense page; treat any such references in the design system as inherited context, not current scope.
- No verdict or settlement dollar figures anywhere — the live site publishes none. `CaseResultCard` exists in the kit but must be used for rating/review-count/availability figures only until Lester supplies verified numbers with the required "past results do not guarantee a similar outcome" footnote.
- Every page needs a full Spanish counterpart per the design system's bilingual requirement (§ Content Fundamentals in the design-system readme) — layouts must hold ~20–25% longer Spanish strings without breaking (see the "Bilingual headline test" guideline card, not yet pulled into this repo).

## Required states
[AI: Define applicable non-happy-path states. Delete irrelevant rows.]

| State | Expected behavior |
|---|---|
| Loading | [expectation] |
| Empty | [expectation] |
| Error | [expectation] |
| Success | [expectation] |
| Restricted | [expectation] |

## Conflicts
If design sources conflict, follow:
1. explicit approved build brief;
2. most specific project-level design instruction;
3. the design-system source identified as canonical.

Do not silently combine contradictory rules. Record consequential resolutions in `06-DECISIONS.md`.
