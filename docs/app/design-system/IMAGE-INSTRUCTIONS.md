# Image Asset Handoff — Nichols Law Group Rebuild
Prepared by DSG. Source: 5 initial page saves (zip format) + 24 additional page saves (self-contained HTML with embedded images), covering effectively the full site including all practice-area sub-pages and policy pages.

**Combined total:** 208 images from batch 1 + 385 embedded image references from batch 2 → after de-duplication across both batches by file content (not filename) → **30 images with a defined use.**

Raw binaries are not checked into this repo — pull them from Google Drive ("Nichols Law Group — DSG Project" → design system export → `assets/`) as each page is implemented. This file is the manifest of what exists and where it's meant to go.

---

## 1. BRAND — `images/brand/`

| File | What it is | Use for |
|---|---|---|
| `logo-primary-horizontal.png` | Full navy wordmark + column/scales icon lockup (800×200 master) | Header, footer |
| `logo-icon-mark-square.png` | Icon-only monogram, navy (680×680 master) | Favicon, app icon, watermark seed |
| `logo-watermark-background.png` | Pale/ghosted full-bleed version of the icon (2000×846) | Section background texture |

No white/reversed-color logo variant exists anywhere across either batch — needed only if the new design uses a dark-background header or hero.

---

## 2. PEOPLE — `images/people/`

| File | Who / what | Use |
|---|---|---|
| `lester-nichols-primary-headshot.png` | **Lester Nichols — proper front-facing professional headshot, suit, transparent background.** Found in batch 2, not visible in the first 5 pages captured. | **This is the primary photo to use** — About page hero, homepage, anywhere a clean headshot is needed. Transparent background means it drops onto any color/section cleanly. |
| `lester-nichols-office-desk.jpg` | Lester at his desk, office with diplomas/bookshelf visible (previously labeled primary — downgraded now that the real headshot above was found) | Secondary/environmental shot — good for a "day in the office" section, not the main headshot slot anymore. |
| `nichols-kids-photo-1-milliana.png` | Lester with daughter Milliana (8) | "The Nichols Kids" section. Live caption: favorite subjects writing & PE, competitive dancer, wants to be a NICU nurse like her mom. |
| `nichols-kids-photo-2-islani.png` | Lester with daughter Islani (3.5) | Same section. Live caption: sings/dances, plays with family dogs, wants to be a veterinarian. |
| `christian-bautista-medical-coordinator.png` | Christian Bautista, the firm's medical coordinator | His own staff bio card. Live caption: tracks all client medical treatment (ER, PT, MRIs) and helps place clients for referred treatment. |

**Note carried forward from the first pass:** the kids' bios are currently more detailed than Lester's own professional bio (still "Bio Coming Soon" — Audit finding A). Finding the real headshot doesn't fix that — a real written bio is still needed. Worth deciding with the client whether to keep the kids section as-is once the professional side is built out properly, not something to unilaterally cut.

---

## 3. GENERAL / SITE-WIDE — `images/general/`

| File | What it is | Use for |
|---|---|---|
| `houston-skyline-hero-background.png` | Houston downtown skyline at dusk, navy color-overlay already applied (2000×1335) | Strong candidate for the homepage hero background or a section divider — matches a navy brand palette already. |
| `gavel-scales-generic-legal.jpg` | Generic gavel/law-book/scales stock shot (400×599) | Appeared on the policy pages (Terms, Privacy, Cookie Policy) — reasonable to reuse there, or as generic filler on any page that doesn't have a specific practice-area image. |

---

## 4. PRACTICE AREA IMAGERY — `images/practice-area/` (20 files)

All generic licensed stock photography. Fine to reuse for launch — no legal issue, no extra cost — but none are differentiated from any competitor's site. Worth flagging to the client as a place to invest in custom/better imagery later, not a launch blocker.

**Original 15 (one per topic):**

| File | Topic | Suggested page/section |
|---|---|---|
| `car-accident-general.jpg` | Car accident (general) | Diminished Value Claims hero |
| `car-accident-near-me.jpg` | Car accident (alt angle) | Motor Vehicle Accidents — car accidents |
| `criminal-defense.jpg` | Break-in / criminal scene | *(Criminal Defense is cut from the rebuilt site's scope per the Master Build Spec — this image has no current page to attach to.)* |
| `distracted-driving.jpg` | Distracted driving | Motor Vehicle Accidents — distracted driving |
| `dog-animal-attack.jpg` | Dog attack | Personal Injury — animal attack |
| `drunk-driving-dui.jpg` | DUI — driver drinking behind wheel | Motor Vehicle Accidents — drunk driving |
| `maritime-offshore.jpg` | Maritime/offshore | Personal Injury — maritime accidents |
| `motorcycle-accident.jpg` | Motorcycle accident | Motor Vehicle Accidents — motorcycle |
| `oilfield-accident.jpg` | Oilfield accident | Personal Injury — oilfield accidents |
| `refinery-accident.jpg` | Refinery accident | Personal Injury — refinery accidents |
| `rideshare-uber-lyft.jpg` | Rideshare accident | Motor Vehicle Accidents — ridesharing |
| `slip-and-fall.jpg` | Slip and fall | Personal Injury — slip & fall |
| `tractor-trailer-accident.jpg` | 18-wheeler/tractor trailer | Motor Vehicle Accidents — tractor trailer |
| `uninsured-underinsured.jpg` | Uninsured motorist | Motor Vehicle Accidents — uninsured/underinsured |
| `wrongful-death.jpg` | Wrongful death | Personal Injury — wrongful death |

Plus `wheelchair-mobility-injury.jpg` and other supplementary practice-area/general images observed in the unzipped Drive folder (e.g. duplicated across subfolders for different page contexts) — see the live Drive folder listing for the full current set; this table reflects the original DSG handoff note and may not be exhaustive of every file actually present.

---

## Note on scope

Per the Master Build Spec (`docs/app/03-DESIGN.md` and the top-level build spec doc), Criminal Defense is cut from the rebuilt site. The `criminal-defense.jpg` asset above is inherited from the original image handoff and currently has no page to attach to — do not build a Criminal Defense page around it.
