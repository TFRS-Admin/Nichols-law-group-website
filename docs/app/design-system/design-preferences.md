# Design preferences — locked in from Nichols Law Group review

These apply to every design system built in this workspace. Read before designing.

## Never do these (generic/AI-slop defaults)
- **No accent color used as a decorative border/stripe repeated across multiple unrelated components** (top-border or left-border accent bars as a default "card" treatment). If an accent rule appears more than once as decoration, it's a tic, not a signature — delete it everywhere except the one true signature element.
- **No soft-drop-shadow + rounded-corner + hairline-border as the default card.** That combo is the generic SaaS/Tailwind template look. Default to flat: hairline border only, or no border at all — let spacing, type scale, and rules carry hierarchy instead of shadow/elevation.
- **No untreated stock photography sitting next to a refined type system.** Generic/illustrative stock imagery (not real people) always gets one consistent grade/overlay applied everywhere it appears (duotone, desaturation + brand-color wash, consistent crop ratio). Real people photos (staff, headshots) stay clean and faithful — never apply the stock grade to them.
- **No more than one accent color used decoratively.** Reserve it for true CTAs/urgency and the one signature element — not for repeating stripes, bullets, icons.
- **No default-tracking/default-weight Google Font used as-is everywhere.** Pick 2–3 deliberate type moves (a specific negative tracking on display type, a distinct tabular-numeral treatment for big figures, a weight contrast rule) and apply them consistently — not just on the hero.
- **No aggressive gradients, neon-on-black, or the generic corporate-blue-and-white SaaS look with no point of view.**

## Favor these (signals of a premium system)
- **One signature element, used exactly once**, tied to the single most important real fact about the brand (not a reusable card style stamped everywhere).
- **Flat, structural hierarchy**: rules, type scale, and whitespace do the separating; shadows and radius are the exception, not the rule.
- **Consistent photographic treatment** across every instance of generic/stock imagery; real people photos stay untouched.
- **Restraint**: max 1–2 background colors across the whole system; one accent, spent deliberately.
- **Real content specificity** over generic copy or invented stats — actual names, numbers, and facts the client can stand behind.

## How to apply
When starting or auditing a design system, check new components against this list before presenting. If a pattern here shows up more than once as decoration, it's wrong — flatten it and reserve any accent treatment for the one true signature moment.

## Type & case (added after Nichols Law Group review 2)
- **No serif display face by default.** Traditional serifs read as generic "law firm" — favor an authoritative sans or a slab with real weight (e.g. Archivo, not Fraunces/Playfair) for headlines.
- **No small-caps "eyebrow" kicker repeated above every section heading.** One kicker per page (e.g. above the hero H1) is fine; the same pattern stamped above every H2 down the page is noise — the heading carries the section alone.
- **Headers and buttons are Title Case, set via authored copy — never forced with `text-transform: uppercase` + letter-spacing.** That CSS pattern is the generic micro-label tic; if a label needs emphasis, use weight/color/size, not case-transform.
- **No monospace font anywhere** unless displaying literal code — not for phone numbers, figures, or labels.
- **Utility icon buttons (menu, language toggle, etc.) shouldn't default to the same bordered square everywhere** — vary the shape/treatment so repeated chrome doesn't read as templated.
- **Card body text needs real editorial structure** (list markers, a closing rule before the CTA, deliberate type-scale steps) — a heading + raw `<li>` text + a floating link is the "no thought" look.
