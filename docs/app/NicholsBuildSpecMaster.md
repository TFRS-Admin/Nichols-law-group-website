# The Nichols Law Group — Master Build Spec (Prototype)
**Prepared by DSG (Dosser Sales Group) · Prototype handoff for Claude Code · August 28, 2026**

This is the single consolidated deliverable: everything Claude Code needs to build the Nichols Law Group prototype site, in one document. It merges the locked project decisions, the finished site copy for all 19 pages, the Blair/Conversation AI build spec, the AEO strategy and pre-publish checklist, and the keyword validation that shaped the copy — so nothing has to be cross-referenced across separate docs during the build.

**This is a prototype, built to show Lester Nichols before the official round.** Placeholders are intentional and ship as-is (flagged inline wherever they appear) — they are not blockers. See §2.

---

## Table of Contents

1. Project State — Locked Decisions
2. Build Sequencing — Prototype vs. Official
3. Sitewide Constants
4. Finished Site Copy — All 19 Pages
5. Blair & Conversation AI Build Spec
6. Website Chat Widget Embed — Ready to Paste
7. AEO Strategy & Pre-Publish Checklist
8. Keyword Validation Summary
9. Open Items — Explicitly Not Blocking This Build

---

## 1. Project State — Locked Decisions

Source of truth: `Nichols-Master-Plan-v2.md`. If anything elsewhere in this project conflicts with the table below, this table wins.

| Decision | Answer |
|---|---|
| Assistant name | **Blair** |
| Blair's three modes | Front Desk (routing) → PI Intake (already built) → Existing Client (assistant-style communication) |
| Conversation AI | Same Blair persona, text/chat-widget + SMS channel, built in parallel |
| Bilingual rollout order | Site gets Spanish first. AI agents (Blair + Conversation AI) follow once site content is finalized |
| Lester packet delivery | Email + logged in HighLevel (both) |
| Website platform | Base44, via Claude Code |
| Website page structure | Individual incident-type pages kept (car, motorcycle, trucking, maritime, oilfield, slip & fall, dog bite, wrongful death, rideshare, etc.), each modernized — not consolidated |
| Website scope | PI-only. Everything non-PI removed. Site is a landing experience feeding the AI intake system |
| Client Portal | Kept, simple: client info + FAQs. No course, no case-management layer |
| Courses | Cut |
| **Criminal Defense** | **Cut** — confirmed 2026-08-28, resolving an earlier scope conflict. `/criminal-defense-lawyer-houston/` should not exist on the rebuilt site |
| Mobile app | Cut |
| Transfer/fallback number for Blair | Still being developed by Travis — not resolved. Post-approval item, not a prototype blocker |
| Recording disclosure language | Still needs attorney (Lester) approval — draft language only. Post-approval item, not a prototype blocker |

**The pitch:** Nichols is going all-in on Personal Injury, pre-litigation, AI-handled. Blair (Voice) and the Conversation AI twin (chat/SMS) run Front Desk routing, a scenario-specific PI consultation, and existing-client communication — one persona, two channels. Every completed intake becomes a decision-ready packet for Lester. *"I handle everything except the case work, so you can scale pre-litigation."*

---

## 2. Build Sequencing — Prototype vs. Official

**Confirmed by Travis:** this build is a prototype to show Lester, not the final ship. That resets what counts as a blocker.

**Not blockers for the prototype — placeholders ship as-is:**
- Lester's real bio → "Bio Coming Soon" / bracketed placeholder stands (Page 2)
- Transfer/fallback number for Blair → escalation nodes stay unwired/stubbed
- Attorney sign-off on recording-disclosure language → draft language ships, unapproved
- Real review-count/case-result figures on Home → `[X]+ five-star reviews` placeholder stands (Page 1)
- Full SEO/AEO polish beyond what's in this doc (unique meta descriptions everywhere, full LegalService/Attorney/Organization schema beyond FAQPage, internal-linking fixes) → shine for the official round, not required to demo credibly

**What the prototype needs, and has, in this doc:** all 19 pages of finished copy, sitewide fixes (phone numbers, live-year footer, DSG credit lockup), the GHL chat widget embed code, and the AEO pre-publish checklist to build against.

**Official round, after Lester sees the prototype and signs off:** real bio, real transfer number, attorney-approved disclosure language, real review numbers, full SEO/AEO/schema/linking polish pass. The prototype's approval is the kickoff of that round, not something running in parallel with it.

---

## 3. Sitewide Constants

Repeat identically across every page.

**Footer:** LESTER NICHOLS LAW — 9408 Cypress Creek Parkway, Houston, Texas 77070 — (713) 705-2250 — (844) NLG-WINS / (844) 654-9467 — Open 24 Hours — © `{current year}` The Nichols Law Group, PLLC — **DosserSales Group | DSG**

- Copyright year is a **live variable**, not hardcoded — render the actual year at page load.
- The DSG credit line replaces "Website Designed & Managed by Above All Media." Paper-on-navy masthead treatment: "Dosser" in brass (`#A6812F` / brass-500, or brass-700 for text weight), "Sales Group" in paper white, brass `| DSG` tail. Libre Franklin 500 (12.5–13px, sentence case, zero letterspacing) or Archivo 600 if treated as a display lockup. Quiet placement, same weight class the old credit line occupied. No gradients, no emoji, no exclamation points, no letterspacing.

**Phone standard, no exceptions:**
- **(713) 705-2250** — local
- **(844) NLG-WINS** / **(844) 654-9467** — toll-free (same number, two presentations both acceptable)
- Do **not** use a standalone "844-654-9467" formatted differently elsewhere — confirmed a duplicate/typo rendering in the source content, already scrubbed from the copy below.

**LegalService/Organization schema:** identical block on every page (see Page 1 for the reference FAQPage pattern to follow) — only `url` changes per page.

---

## 4. Finished Site Copy — All 19 Pages

Progress: **19 of 19 pages complete.** Criminal Defense Lawyer Houston is cut from scope (§1, §9 below). Diminished Value Claims stays — nothing ever called for cutting it. Every page below is final copy, ready to build from — not a brief, not a draft.

### PAGE 1 of 19 — Home (`/`)

**Meta title:** Houston Personal Injury Lawyer | The Nichols Law Group, PLLC
**Meta description:** Injured in Houston? The Nichols Law Group fights insurance companies so you don't have to. Free consultation, no fee unless we win. Call (713) 705-2250.
**URL:** `/`
**Target keywords:** Houston personal injury lawyer (primary) · Houston accident attorney, car accident lawyer Houston (secondary)

#### H1: The Nichols Law Group, PLLC — Houston Personal Injury Lawyer

**Hero**
Life Moves Fast and Accidents Happen. When a car accident, workplace injury, or negligent property owner upends your life, The Nichols Law Group gets to work — no fee unless we win.

[Get a FREE Consultation] [Call (713) 705-2250]

#### Why Hire a Houston Personal Injury Lawyer?

Insurance companies employ teams of adjusters and attorneys whose job is to pay you as little as possible — hiring a Houston personal injury lawyer puts someone in your corner with the same leverage. The Nichols Law Group handles the insurance fight, the paperwork, and the deadlines so you can focus on recovering.

The right time to call is immediately after an accident, not after you've already spoken with an insurance adjuster. Evidence disappears, memories fade, and Texas' filing deadlines don't pause for you to figure out your next step.

*What to look for in a Houston personal injury attorney:* trial-readiness (not just settlement experience), a track record with your type of case, and real client reviews — [X]+ five-star Google reviews. **[Placeholder — real review count needed from Lester, official round only.]**

#### How We Help — Auto Accidents & Personal Injury

**Auto Accidents:** Car Accidents · Trucking Accidents (18-Wheelers) · Motorcycle Accidents · Drunk Driving Accidents · Distracted Driver Accidents · Uninsured Motorist Claims · Uber & Lyft Accidents

**Personal Injury:** Dog Bites & Animal Attacks · Maritime Accidents · Oilfield Accidents · Slip & Fall Accidents · Wrongful Death · Refinery Accidents

*(No Criminal Defense grid link — cut from scope, see §1/§9.)*

#### What Happens After You Call?

Your first call gets you a free, no-obligation case review. Once retained, our team investigates your accident, coordinates with your medical providers, and handles every insurance conversation so adjusters stop calling you directly. Christian Bautista, our in-house medical coordinator, tracks your treatment and helps you find care even if you don't have insurance of your own.

#### FAQ
**How long does a case take?** Straightforward claims can resolve in a few months; disputed or serious-injury cases can take a year or more.
**What can I recover?** Medical expenses, lost wages and earning capacity, property damage, pain and suffering, and in gross-negligence cases, punitive damages.
**Do I pay anything upfront?** No — contingency fee, nothing unless we win.
**What if my accident was outside Houston proper?** We cover greater Houston and Harris County, including I-45, I-10, 610 Loop cases, plus maritime/offshore claims tied to the Port of Houston and Gulf Coast oilfield accidents.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen. [Reach Out For a FREE Consultation]

**Placeholders flagged:** [X]+ five-star reviews and any years-in-practice/case-result stats need real figures from Lester — official round, not fabricated here.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"How long does a personal injury case take to resolve?","acceptedAnswer":{"@type":"Answer","text":"Straightforward claims can resolve in a few months; cases involving serious injury, disputed fault, or a reluctant insurer can take a year or more."}},
{"@type":"Question","name":"What compensation can I recover?","acceptedAnswer":{"@type":"Answer","text":"Medical expenses, lost wages and diminished earning capacity, property damage, pain and suffering, and in gross-negligence cases, punitive damages."}},
{"@type":"Question","name":"Do I have to pay anything upfront?","acceptedAnswer":{"@type":"Answer","text":"No. The Nichols Law Group works on contingency — nothing upfront, nothing unless we win."}},
{"@type":"Question","name":"What if the accident happened outside Houston proper?","acceptedAnswer":{"@type":"Answer","text":"We represent clients throughout greater Houston and Harris County, including I-45, I-10, and 610 Loop cases, plus maritime and oilfield claims across the Gulf Coast."}}
]}
```

---

### PAGE 2 of 19 — About Us (`/about-us/`)

**Meta title:** About The Nichols Law Group | Houston Personal Injury Attorneys
**Meta description:** Meet the team at The Nichols Law Group — a Houston personal injury firm built around real client care, from first call to final resolution.
**Target keywords:** Lester Nichols attorney Houston (primary) · Nichols Law Group about (secondary)

#### H1: About The Nichols Law Group

**Lester Nichols** — [Bio placeholder — needs real input from Lester, official round. Do not launch officially with a placeholder; fine for the prototype.] [Call (713) 705-2250]

#### Family and Firm
Lester balances the practice with raising two kids who are already lawyers-in-training, by their own account. Milliana, 8, dances competitively and currently plans on becoming a NICU nurse like her mom. Islani, 3.5, sings and dances with the family and wants to be a veterinarian.

#### Christian Bautista — Medical Coordinator
If you're in pain after an accident, Christian is often the first person on our team you'll talk to. He tracks every step of your medical care — ER visits, physical therapy, imaging — and helps connect you with providers even without insurance of your own.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen. [Reach Out For a FREE Consultation]

---

### PAGE 3 of 19 — Contact Us (`/contact-us/`)

**Meta title:** Contact The Nichols Law Group | Free Houston Injury Consultation
**Meta description:** Reach The Nichols Law Group 24/7 for a free personal injury consultation. Call, text, or send your case details — we respond fast.
**Target keywords:** contact Houston personal injury lawyer

#### H1: Contact Our Houston Lawyer

**Ask About Our Free Consultation** — Whether you were just in an accident or you're still deciding if you have a case, reaching out costs nothing. Call, text, or fill out the form below and a member of our team will follow up personally.

**Contact Info:** (844) NLG-WINS · (713) 705-2250 · 9408 Cypress Creek Parkway, Houston, Texas 77070 · Open 24 Hours

**Confirmation text (fixed, client-facing):** "Thank you for reaching out to The Nichols Law Group. We've received your information and a member of our team will contact you shortly. If your matter is urgent, please call us directly at (713) 705-2250."

**Disclaimer:** Any information you obtain from this site is not legal advice, nor is it intended to be. Consult an attorney for advice regarding your individual situation.

---

### PAGE 4 of 19 — Motor Vehicle Accidents (hub) (`/motor-vehicle-accidents/`)

**Meta title:** Houston Car Accident Lawyer | Motor Vehicle Accident Attorney
**Meta description:** The Nichols Law Group represents Houston drivers, passengers, motorcyclists, and rideshare riders after any motor vehicle accident. Free consultation.
**Target keywords:** Houston car accident lawyer (primary) · Houston auto accident attorney (secondary)

#### H1: Motor Vehicle Accident Attorney

A motor vehicle accident claim covers any collision involving a car, truck, motorcycle, or rideshare vehicle — the right attorney for your case depends on what caused the crash and what kind of vehicle was involved, which is why we handle each accident type as its own specialty rather than one generic "car accident" claim.

**Car Accidents** — Standard passenger-vehicle collisions, from rear-end crashes to multi-car pileups on I-10 or the 610 Loop.
**Uninsured Motorist Claims** — When the at-fault driver has no insurance or not enough to cover your damages.
**18-Wheeler Accidents** — Commercial trucking cases involve FMCSA regulations and multiple potentially liable parties beyond the driver.
**Motorcycle Accidents** — Motorcyclists face different injury severity and different bias from insurers than car drivers.
**Drunk Driving Accidents** — Cases against intoxicated drivers, which can support both civil claims and criminal consequences.
**Distracted Driving Accidents** — Texting-and-driving and other distraction-caused crashes, increasingly common on Houston's busiest corridors.
**Uber & Lyft Accidents** — Rideshare cases involve layered insurance coverage that depends on whether the driver was logged into the app.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen. [Reach Out For a FREE Consultation]

---

### PAGE 5 of 19 — Personal Injury (hub) (`/personal-injury/`)

**Meta title:** Houston Personal Injury Lawyer | Personal Injury Practice Areas
**Meta description:** From dog bites to oilfield accidents, The Nichols Law Group handles Houston personal injury claims outside of standard car accidents. Free consultation.
**Target keywords:** Houston personal injury lawyer (primary) · Houston injury attorney (secondary)

#### H1: Houston's Top-Rated Personal Injury Lawyer

Personal injury covers any case where someone else's negligence caused you harm outside a standard car accident — animal attacks, maritime and offshore incidents, industrial accidents, dangerous property conditions, and wrongful death. Each area below has its own legal standards and evidence requirements.

**Dog & Animal Attacks** — Texas premises-liability and owner-responsibility law after a bite or attack.
**Maritime Accident Lawyer** — Offshore and Port of Houston-area incidents governed by admiralty law, not standard state injury law.
**Refinery Accidents** — Injuries at Houston's refineries and petrochemical plants, often involving multiple corporate parties.
**Slip & Fall Accidents** — Injuries caused by a property owner's failure to maintain safe conditions.
**Wrongful Death** — Claims brought by surviving family after a fatal accident caused by negligence.
**Oilfield Accidents** — Injuries in one of the most hazardous sectors in the Houston economy, from drilling sites to fracking operations.

*(All six links resolve to live pages — none should point to `#`.)*

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen. [Reach Out For a FREE Consultation]

---

### PAGE 6 of 19 — Car Accidents Lawyer (`/motor-vehicle-accidents/car-accidents-lawyer/`)

**Meta title:** Houston Car Accident Lawyer | The Nichols Law Group
**Meta description:** Injured in a Houston car accident? The Nichols Law Group handles the insurance fight so you can focus on recovery. Free consultation, no fee unless we win.
**Target keywords:** Houston car accident lawyer (primary) · car accident attorney Houston TX (secondary)

#### H1: Car Accidents Lawyer

**What should I do after a Houston car accident?** Seek medical attention first, then gather evidence — photos of the scene, the other driver's information, and a copy of the police report — before you speak with any insurance company, including your own.

**Filing a Personal Injury Insurance Claim** — Track every medical bill, day of missed work, and repair estimate from day one; insurers routinely undervalue claims that arrive without documentation. We gather evidence, contact the right parties, and file the report so nothing gets missed.

**Common Causes of Houston Car Accidents:** drunk driving, speeding on highways like I-45 and the 610 Loop, distracted driving, failure to yield, running red lights, and improper turns at high-traffic intersections.

**Looking for a car accident attorney?** Choose a firm with real trial experience, a track record with cases like yours, and reviews from actual past clients — not just marketing claims.

#### FAQ
**How long do I have to file a claim in Texas?** Generally two years from the date of the accident for personal injury claims, though exceptions can shorten or extend that window — don't wait to find out which applies to you.
**What if I was partially at fault?** Texas follows modified comparative negligence — you can still recover if you're less than 51% at fault, though your recovery is reduced by your share of fault.

#### Closing CTA
Reach Out For a FREE Consultation.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"How long do I have to file a car accident claim in Texas?","acceptedAnswer":{"@type":"Answer","text":"Generally two years from the date of the accident, though certain circumstances can shorten or extend that window."}},
{"@type":"Question","name":"What if I was partially at fault for the accident?","acceptedAnswer":{"@type":"Answer","text":"Texas follows modified comparative negligence — you can still recover damages if you're less than 51% at fault, though your recovery is reduced by your share of fault."}}
]}
```

---

### PAGE 7 of 19 — Distracted Driving Accident Lawyer (`/motor-vehicle-accidents/distracted-driving-accident-lawyer/`)

**Meta title:** Houston Distracted Driving Accident Lawyer | The Nichols Law Group
**Meta description:** Hit by a distracted driver in Houston? The Nichols Law Group builds the case insurers can't ignore. Free consultation, no fee unless we win.
**Target keywords:** Houston distracted driving accident lawyer (primary) · texting and driving accident attorney Houston (secondary)

#### H1: Distracted Driving Accident Lawyer

**What counts as distracted driving in Texas?** Texting behind the wheel is illegal statewide under Texas Transportation Code §545.4251 — but distraction also covers phone calls, eating, GPS use, and anything that takes a driver's attention off the road long enough to miss a hazard.

**Hit by a distracted driver? What to do next:** stay calm, seek medical attention if injured, and avoid giving a recorded statement to any insurance company before speaking with an attorney — insurers are looking out for their own interests, not yours.

**Filing an insurance claim:** we handle the claim regardless of who's found at fault initially, and pursue a rental car and reimbursement for lost wages and medical expenses while your case is pending.

#### FAQ
**Is texting and driving illegal in Houston?** Yes — Texas law bans reading, writing, or sending texts while driving statewide, and Houston enforces it actively on major corridors.
**Can I still recover damages if there's no ticket issued?** Yes — a citation helps but isn't required; phone records, witness statements, and crash reconstruction can establish distraction independently.

#### Closing CTA
Get a FREE Consultation.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Is texting and driving illegal in Houston?","acceptedAnswer":{"@type":"Answer","text":"Yes. Texas law bans reading, writing, or sending texts while driving statewide, and Houston enforces it actively on major corridors."}},
{"@type":"Question","name":"Can I still recover damages if no ticket was issued?","acceptedAnswer":{"@type":"Answer","text":"Yes. A citation helps but isn't required — phone records, witness statements, and crash reconstruction can establish distraction independently."}}
]}
```

---

### PAGE 8 of 19 — Drunk Driving Accident Lawyer (`/motor-vehicle-accidents/drunk-driving-accident-lawyer/`)

**Meta title:** Houston Drunk Driving Accident Lawyer | The Nichols Law Group
**Meta description:** Injured by a drunk driver in Houston? The Nichols Law Group pursues full compensation while any criminal case runs separately. Free consultation.
**Target keywords:** Houston drunk driving accident lawyer (primary) · DUI accident attorney Houston (secondary)

#### H1: Drunk Driving Accident Lawyer

**Hit by a drunk driver? What to do next:** seek medical attention, get the police report (which will typically include any BAC or field sobriety findings), and avoid direct communication with the at-fault driver's insurer.

**Filing an insurance claim after a DWI crash:** we obtain the driver's insurance information and policy details, document everything, and contact insurers promptly — a criminal DWI conviction doesn't automatically resolve your civil claim, and the two proceed separately.

**Need a drunk driving accident attorney?** Cases involving intoxication often support higher damages, including punitive damages in Texas when gross negligence is shown.

#### FAQ
**Does the criminal DWI case affect my civil claim?** They run on separate tracks — a criminal conviction can strengthen a civil case, but you don't have to wait for it to resolve before pursuing compensation.
**Can I recover punitive damages?** Texas allows punitive damages in cases involving gross negligence or malice, which drunk driving cases can meet depending on the facts.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen. Reach Out For a FREE Consultation.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Does the criminal DWI case affect my civil claim?","acceptedAnswer":{"@type":"Answer","text":"They run on separate tracks. A criminal conviction can strengthen a civil case, but you don't have to wait for it to resolve before pursuing compensation."}},
{"@type":"Question","name":"Can I recover punitive damages in a drunk driving case?","acceptedAnswer":{"@type":"Answer","text":"Texas allows punitive damages in cases involving gross negligence or malice, which drunk driving cases can meet depending on the facts."}}
]}
```

---

### PAGE 9 of 19 — Motorcycle Accidents Lawyer (`/motor-vehicle-accidents/motorcycle-accidents-lawyer/`)

**Meta title:** Houston Motorcycle Accident Lawyer | The Nichols Law Group
**Meta description:** Motorcycle accident in Houston? Insurers treat riders differently — The Nichols Law Group fights that bias. Free consultation, no fee unless we win.
**Target keywords:** Houston motorcycle accident lawyer (primary) · motorcycle crash attorney Houston (secondary)

#### H1: Motorcycle Accidents Lawyer

**Why do motorcycle accident cases need a specialized approach?** Insurers frequently assume riders share fault by default — a bias that isn't supported by Texas law and that a firm experienced in motorcycle cases knows how to counter with evidence: photos, witness statements, and the police report.

**Common causes:** driver inexperience, impairment, unsafe roads or weather, and drivers simply failing to see a motorcycle in traffic — a documented, common cause of Houston motorcycle collisions.

**How we help:** establishing fault against rider-bias, pursuing full compensation for injury severity that's often worse than car-accident injuries, negotiating directly with insurers, and supporting you through the emotional impact of a serious crash.

#### FAQ
**Do I have to have been wearing a helmet to file a claim?** No — Texas doesn't require a helmet for riders over 21 with proper insurance/training, and a lack of helmet doesn't bar your claim, though it may be raised on damages depending on the injury.
**Why do insurers offer less for motorcycle claims?** Bias, not law — riders are statistically more likely to be blamed by adjusters regardless of fault, which is exactly the assumption a well-documented case pushes back on.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Do I need to have been wearing a helmet to file a motorcycle accident claim?","acceptedAnswer":{"@type":"Answer","text":"No. Texas doesn't require a helmet for riders over 21 with proper insurance and training, and a lack of helmet doesn't bar your claim, though it may be raised on damages depending on the injury."}},
{"@type":"Question","name":"Why do insurers often offer less for motorcycle accident claims?","acceptedAnswer":{"@type":"Answer","text":"Adjusters are statistically more likely to assume riders share fault regardless of the actual facts — a well-documented case pushes back on that assumption directly."}}
]}
```

---

### PAGE 10 of 19 — Ridesharing Lawyer (`/motor-vehicle-accidents/ridesharing-lawyer/`)

**Meta title:** Houston Uber Accident Lawyer | Rideshare Accident Attorney
**Meta description:** Injured in an Uber or Lyft accident in Houston? Rideshare insurance is layered and complicated — The Nichols Law Group sorts it out. Free consultation.
**Target keywords:** Houston Uber accident lawyer (primary) · Lyft accident attorney Houston (secondary)

#### H1: Ridesharing Accident Lawyer

**Why is a rideshare accident claim different from a regular car accident claim?** Whether Uber or Lyft's $1 million liability policy applies depends on the driver's app status at the moment of the crash — logged off, waiting for a ride request, or actively en route — and each status triggers different, layered insurance coverage that a standard car-accident approach won't correctly navigate.

**How we help:** we determine which coverage layer applies to your specific accident, pursue the rideshare company's commercial policy where it applies rather than settling for the driver's personal minimum coverage, and handle every step of the claim on a free-consultation, no-fee-unless-we-win basis.

#### FAQ
**Am I covered if I was a passenger in the Uber?** Generally yes — Uber and Lyft's commercial coverage typically applies to passengers regardless of who caused the crash, though the specific insurer and amount depend on the driver's app status.
**What if the rideshare driver wasn't logged into the app?** Then only their personal auto policy applies, not the company's commercial coverage — a critical distinction that affects how much compensation is actually available.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Am I covered if I was a passenger in an Uber or Lyft accident?","acceptedAnswer":{"@type":"Answer","text":"Generally yes — the rideshare company's commercial coverage typically applies to passengers regardless of fault, though the specific insurer and amount depend on the driver's app status at the time."}},
{"@type":"Question","name":"What if the rideshare driver wasn't logged into the app when the accident happened?","acceptedAnswer":{"@type":"Answer","text":"Then only the driver's personal auto policy applies, not the rideshare company's commercial coverage — a distinction that significantly affects how much compensation is available."}}
]}
```

---

### PAGE 11 of 19 — Tractor Trailer Accidents Lawyer (`/motor-vehicle-accidents/tractor-trailer-accidents-lawyer/`)

**Meta title:** Houston Truck Accident Lawyer | 18-Wheeler Accident Attorney
**Meta description:** Injured in a Houston 18-wheeler accident? Trucking cases involve federal regulations and multiple liable parties. Free consultation.
**Target keywords:** Houston truck accident lawyer (primary — swapped from "18-wheeler accident lawyer" per keyword validation, ~26x higher search volume; see §8) · Houston 18-wheeler accident lawyer (secondary)

#### H1: Truck Accident Lawyer

**What makes an 18-wheeler accident case different from a standard car accident claim?** Commercial trucking is governed by FMCSA (Federal Motor Carrier Safety Administration) regulations covering driver hours, vehicle maintenance, and cargo loading — meaning liability can extend beyond the driver to the trucking company, a maintenance contractor, or a cargo loader.

**Choosing a truck accident attorney:** look for someone who can respond quickly to preserve evidence at the scene, has real personal injury trial experience, and understands commercial trucking insurance — which operates very differently from standard auto policies and often involves much higher coverage limits.

**Common causes:** speeding (not every truck has a speed limiter installed), driver distraction, and aggressive driving from drivers under pressure from long hours and delivery deadlines — tailgating, unsafe passing, and cutting off smaller vehicles.

#### FAQ
**Who can be held liable in an 18-wheeler accident?** Potentially the driver, the trucking company, a maintenance contractor, or whoever loaded the cargo — commercial trucking cases often involve more than one liable party.
**Why do truck accident cases move faster on evidence than car accidents?** Trucking companies are required to preserve certain records (driver logs, black box data) for limited periods — getting an attorney involved quickly protects that evidence before it's gone.

#### Closing CTA
Reach Out For a FREE Consultation.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Who can be held liable in an 18-wheeler accident?","acceptedAnswer":{"@type":"Answer","text":"Potentially the driver, the trucking company, a maintenance contractor, or whoever loaded the cargo — commercial trucking cases often involve more than one liable party."}},
{"@type":"Question","name":"Why is evidence preservation especially urgent in truck accident cases?","acceptedAnswer":{"@type":"Answer","text":"Trucking companies are only required to preserve certain records, like driver logs and black box data, for limited periods — getting an attorney involved quickly protects that evidence before it's gone."}}
]}
```

---

### PAGE 12 of 19 — Uninsured & Underinsured Claims Law Firm (`/motor-vehicle-accidents/uninsured-underinsured-claims-law-firm/`)

**Meta title:** Houston Uninsured Motorist Lawyer | Underinsured Claims Attorney
**Meta description:** Hit by an uninsured or underinsured driver in Houston? Your own policy may still cover you. The Nichols Law Group handles the claim. Free consultation.
**Target keywords:** Houston uninsured motorist lawyer (primary) · underinsured motorist claim attorney Houston (secondary)

#### H1: Uninsured & Underinsured Claims Law Firm

**What is uninsured/underinsured motorist (UM/UIM) coverage?** It's the portion of your own auto policy that pays out when the at-fault driver either has no insurance or doesn't carry enough to cover your damages — a common gap in Texas, where the state doesn't require every driver to carry adequate coverage.

**What to do if you're in an accident with an uninsured driver:** file a claim with your own insurer under your UM/UIM coverage, track every expense from the start, and consider an attorney — your own insurance company still has an incentive to minimize what it pays, even though you're the policyholder.

**Why hire an attorney for a claim against your own insurer?** Because it's still an adversarial claim. We handle every insurer conversation so you're not negotiating alone against a company motivated to pay less.

#### FAQ
**Does Texas require drivers to carry UM/UIM coverage?** Insurers must offer it, but drivers can decline it in writing — many don't realize they've waived it until they need it.
**Can I still recover if the at-fault driver has some insurance, just not enough?** Yes — that's underinsured motorist coverage specifically, and it fills the gap between what their policy pays and your actual damages.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Does Texas require drivers to carry uninsured/underinsured motorist coverage?","acceptedAnswer":{"@type":"Answer","text":"Insurers must offer it, but drivers can decline it in writing — many don't realize they've waived it until they need it."}},
{"@type":"Question","name":"Can I recover if the at-fault driver has insurance but not enough?","acceptedAnswer":{"@type":"Answer","text":"Yes — that's underinsured motorist coverage specifically, and it fills the gap between what their policy pays and your actual damages."}}
]}
```

---

### PAGE 13 of 19 — Animal Attack Lawyer (`/personal-injury/animal-attack-lawyer/`)

**Meta title:** Houston Dog Bite Lawyer | Animal Attack Attorney
**Meta description:** Bitten or attacked by an animal in Houston? The Nichols Law Group pursues the owner's liability for your injuries. Free consultation.
**Target keywords:** Houston dog bite lawyer (primary) · animal attack attorney Houston (secondary)

#### H1: Animal Attack Lawyer

**Who is responsible after a dog bite or animal attack in Houston?** Typically the animal's owner, under Texas premises-liability and negligence principles — though other parties, like a property owner or a business where the attack occurred, can share liability depending on the circumstances.

**How we help:** negotiating directly with the owner's homeowner's or renter's insurance, gathering medical records and documentation of the attack, and timing the claim to maximize your recovery rather than settling too early.

#### FAQ
**What should I do immediately after a dog bite?** Get medical attention, photograph the injury and the scene, get the owner's contact and insurance information if possible, and report the bite to local animal control.
**My child was bitten — what's different?** The same liability principles apply, but documentation matters even more, since a child's injury and its long-term effects may not be fully clear right away.
**How long after the incident can I file a claim?** Generally two years under Texas's personal injury statute of limitations, though the clock can start differently depending on the facts — don't wait to find out.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"What should I do immediately after a dog bite in Houston?","acceptedAnswer":{"@type":"Answer","text":"Get medical attention, photograph the injury and the scene, get the owner's contact and insurance information if possible, and report the bite to local animal control."}},
{"@type":"Question","name":"How long after the incident can I file an animal attack claim in Texas?","acceptedAnswer":{"@type":"Answer","text":"Generally two years under Texas's personal injury statute of limitations, though the clock can start differently depending on the facts."}}
]}
```

---

### PAGE 14 of 19 — Maritime Accident Lawyer (`/personal-injury/maritime-accident-lawyer/`)

**Meta title:** Houston Maritime Accident Lawyer | Admiralty Law Attorney
**Meta description:** Injured offshore or on the water near Houston? Maritime cases fall under admiralty law, not standard state injury law. Free consultation.
**Target keywords:** Houston maritime accident lawyer (primary) · admiralty law attorney Houston (secondary)

#### H1: Maritime Accident Lawyer

**Why do maritime accidents need a specialized attorney?** Incidents that happen on navigable water — including Port of Houston and Gulf Coast offshore work — fall under federal admiralty and maritime law rather than standard Texas personal injury law, with its own compensation rules and filing procedures.

**What compensation is available in a maritime claim?** Medical expenses, lost wages and earning capacity, pain and suffering, physical impairment, disfigurement, and emotional distress — categories that track differently than a standard state injury claim.

**Maritime wrongful death claims:** these require the estate's personal representative to have probate court authority to file, and can recover for loss of support, loss of services, lost inheritance prospects, and burial expenses.

#### FAQ
**Does my injury have to happen literally on a boat to count as maritime?** No — it needs to happen on navigable water or in the course of maritime employment, which covers Port of Houston dock work and offshore oilfield-adjacent incidents too.
**Who can file a maritime wrongful death claim?** The estate's personal representative, appointed through probate court, on behalf of the surviving family.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Does an injury have to happen on a boat to count as a maritime claim?","acceptedAnswer":{"@type":"Answer","text":"No. It needs to happen on navigable water or in the course of maritime employment, which covers Port of Houston dock work and offshore oilfield-adjacent incidents too."}},
{"@type":"Question","name":"Who can file a maritime wrongful death claim?","acceptedAnswer":{"@type":"Answer","text":"The estate's personal representative, appointed through probate court, on behalf of the surviving family."}}
]}
```

---

### PAGE 15 of 19 — Refinery Accident Lawyer (`/personal-injury/refinery-accident-lawyer/`)

**Meta title:** Houston Refinery Accident Lawyer | Refinery Explosion Attorney
**Meta description:** Injured in a Houston-area refinery accident? Cases often involve multiple corporate parties. The Nichols Law Group sorts out liability. Free consultation.
**Target keywords:** Houston refinery accident lawyer (primary) · refinery explosion attorney Houston (secondary)
**Note:** the old page builder's 3 dead fragment-anchor links are replaced with normal in-page navigation in this rebuild — no fragment IDs to preserve.

#### H1: Refinery Accident Lawyer

**Why do refinery accident cases need experienced representation?** Houston's refineries and petrochemical plants often involve multiple entities — the plant operator, a maintenance contractor, an equipment manufacturer — and injured workers frequently find their employer unresponsive once a claim is filed.

**What we bring:** experience with the specific hazards of refinery work, skill in both negotiation and trial-readiness (most cases settle, but insurers negotiate differently with a firm prepared to go to trial), and responsiveness — an attorney who's actually reachable while you recover.

#### FAQ
**Is the refinery company automatically liable for my injury?** Not automatically — liability depends on whether negligence (equipment failure, inadequate safety protocols, insufficient training) caused the accident, which is why documentation matters.
**How much does it cost to hire a refinery accident lawyer?** Nothing upfront — we work on contingency, meaning you pay only if we recover compensation for you.
**Can I file a lawsuit if I already received workers' comp?** Depending on the circumstances, a third-party claim against a contractor or equipment manufacturer may still be available even after workers' comp — worth a free consultation to check.

#### Closing CTA
Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Is the refinery company automatically liable for a worker's injury?","acceptedAnswer":{"@type":"Answer","text":"Not automatically — liability depends on whether negligence, such as equipment failure or inadequate safety protocols, caused the accident."}},
{"@type":"Question","name":"How much does it cost to hire a refinery accident lawyer?","acceptedAnswer":{"@type":"Answer","text":"Nothing upfront. The Nichols Law Group works on contingency, meaning you pay only if compensation is recovered."}}
]}
```

---

### PAGE 16 of 19 — Slip and Fall Lawyer (`/personal-injury/slip-and-fall-lawyer/`)

**Meta title:** Houston Slip and Fall Lawyer | Premises Liability Attorney
**Meta description:** Injured in a Houston slip and fall? Property owners have a legal duty to keep conditions safe. The Nichols Law Group holds them to it. Free consultation.
**Target keywords:** Houston slip and fall lawyer (primary) · premises liability attorney Houston (secondary)

#### H1: Slip and Fall Lawyer

**Can a slip and fall really cause a serious injury?** Yes — hip fractures, head injuries, and spinal injuries are common outcomes of what looks like a minor fall, which is exactly why property owners' insurers try to minimize these claims early.

**How we help:** establishing that the property owner knew or should have known about the hazardous condition, preventing you from agreeing to an unfair early settlement before you know the full extent of your injuries, and representing you at trial if the insurer won't offer a fair number.

#### FAQ
**What does a property owner have to prove they did to avoid liability?** Under Texas premises-liability law, they must show reasonable care in maintaining the property and warning of known hazards — failing that standard is what creates liability.
**Do I need proof the owner knew about the hazard?** Generally yes, actual or constructive knowledge (they should have known through reasonable inspection) is a required element of a Texas slip-and-fall claim.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"What must a property owner prove to avoid liability in a Texas slip and fall case?","acceptedAnswer":{"@type":"Answer","text":"Reasonable care in maintaining the property and warning of known hazards — failing that standard is what creates liability."}},
{"@type":"Question","name":"Do I need to prove the owner knew about the hazard?","acceptedAnswer":{"@type":"Answer","text":"Generally yes — actual or constructive knowledge, meaning they knew or should have known through reasonable inspection, is a required element of a Texas slip-and-fall claim."}}
]}
```

---

### PAGE 17 of 19 — Wrongful Death Lawyer (`/personal-injury/wrongful-death-lawyer/`)

**Meta title:** Houston Wrongful Death Lawyer | Wrongful Death Attorney
**Meta description:** Lost a family member to someone else's negligence in Houston? The Nichols Law Group pursues accountability and compensation. Free consultation.
**Target keywords:** Houston wrongful death lawyer (primary) · wrongful death attorney Houston TX (secondary)

#### H1: Wrongful Death Lawyer

**Who can sue for wrongful death in Texas?** The deceased's surviving spouse, children, and parents may file directly; if they don't file within three months, the estate's personal representative can file on the family's behalf.

**What are the time limits?** Texas generally allows two years from the date of death to file a wrongful death claim, though certain circumstances can affect that deadline — an attorney can confirm your specific timeline early.

**What is a wrongful death case worth?** Recoverable damages include medical costs incurred before death, lost income and financial support, funeral and burial expenses, and the family's pain and suffering — the specific value depends heavily on the facts of the case.

#### FAQ
**How do I find the right wrongful death lawyer?** Look for real experience with wrongful death cases specifically, genuine empathy for what your family is going through, and a firm's actual reputation with past clients — not just advertising.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"Who can sue for wrongful death in Texas?","acceptedAnswer":{"@type":"Answer","text":"The deceased's surviving spouse, children, and parents may file directly. If they don't file within three months, the estate's personal representative can file on the family's behalf."}},
{"@type":"Question","name":"What is the time limit for filing a wrongful death case in Texas?","acceptedAnswer":{"@type":"Answer","text":"Generally two years from the date of death, though certain circumstances can affect that deadline."}}
]}
```

---

### PAGE 18 of 19 — Oilfield Law Firm (`/personal-injury/oilfield-law-firm/`)

**Meta title:** Houston Oilfield Accident Lawyer | Oilfield Injury Attorney
**Meta description:** Injured in a Houston-area oilfield accident? One of the most hazardous industries deserves an attorney who knows it. Free consultation.
**Target keywords:** Houston oilfield accident lawyer (primary) · oilfield injury attorney Houston (secondary)

#### H1: Houston Oilfield Accident Lawyer

**Why is oilfield work one of the most dangerous jobs in Houston?** Between equipment malfunctions, explosions and fires, falls, fracking mishaps and blowouts, and confined-space incidents, hundreds of Houston-area oil and gas workers are injured every year — and drilling-site risk means a serious accident is always a real possibility, not a remote one.

**How do I know if I have a case?** It depends on the nature of your injury, whether negligence (not just an unavoidable accident) played a role, the extent of your injuries, and your medical expenses — a free consultation is the fastest way to find out.

#### FAQ
**What compensation can I expect from an oilfield accident claim?** Medical expenses, lost wages, pain and suffering, and other damages depending on the case — most oilfield accident cases resolve within one to two years.
**What are the most common causes of oilfield accidents?** Equipment failure or malfunction, explosions and fires, falls, fracking mishaps and blowouts, and workers becoming trapped or confined.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. Life Moves Fast And Accidents Happen.

**FAQPage schema:**
```json
{"@context":"https://schema.org","@type":"FAQPage","mainEntity":[
{"@type":"Question","name":"What compensation can I expect from an oilfield accident claim?","acceptedAnswer":{"@type":"Answer","text":"Medical expenses, lost wages, pain and suffering, and other damages depending on the case. Most oilfield accident cases resolve within one to two years."}},
{"@type":"Question","name":"What are the most common causes of oilfield accidents?","acceptedAnswer":{"@type":"Answer","text":"Equipment failure or malfunction, explosions and fires, falls, fracking mishaps and blowouts, and workers becoming trapped or confined."}}
]}
```

---

### PAGE 19 of 19 — Diminished Value Claims (`/diminished-value/`)

**Meta title:** Houston Diminished Value Claim | Diminished Value Lawyer Texas
**Meta description:** Your car's resale value dropped after an accident, even with perfect repairs. The Nichols Law Group pursues that loss too. Free consultation.
**Target keywords:** Houston diminished value claim (primary) · diminished value lawyer Texas (secondary)

#### H1: Diminished Value Claims

**What is a diminished value claim?** Even after perfect repairs, a vehicle that's been in an accident is worth less on resale than one with a clean history — Texas law allows you to claim that lost value separately from your repair costs, and insurers routinely deny or minimize these claims because most people don't know to ask.

**A worked example:** a one-year-old vehicle worth $30,000 sustains $5,000 in accident damage. Even with a flawless repair, its resale value may drop to around $22,000 — an $8,000 diminished value loss that repair costs alone never account for.

**Already settled the repair claim?** You can still file a diminished value claim separately, even after body-damage repairs are complete — the question is whether your own insurer or the at-fault driver's insurer is responsible for that payout, which depends on the specifics of your accident.

#### Closing CTA
Contact Our Expert Personal Injury Attorney Today. [Reach Out For a FREE Consultation]

---

### CUT FROM SCOPE — Criminal Defense Lawyer Houston

`/criminal-defense-lawyer-houston/` — removed 2026-08-28, matching Master Plan v2's locked "Criminal Defense: Cut" decision. No copy carries forward; the URL should not exist on the rebuilt site, and there is no Home page grid link to it (see Page 1).

---

## 5. Blair & Conversation AI Build Spec

This is the buildable spec for the two real gaps in Blair (Front Desk, Existing Client) plus the Conversation AI twin — written to paste directly into HighLevel's Voice Flow builder and Conversation AI builder. It does **not** recreate the PI intake — that flow (KB `kpQgrfpDkFkSaL83j64i`, 53 fields, the 10-stage pipeline) already exists and stays exactly as-is. This connects a front door and an existing-client mode around it.

English only. Spanish is phase 2, sequenced after the website's Spanish content.

### 5.1 How the Pieces Connect

```
Inbound call/chat
      │
      ▼
  BLAIR — FRONT DESK  (new)
      │
      ├─→ New PI prospect ──→ BLAIR — PI INTAKE  (already built, untouched)
      │                              │
      │                              ▼
      │                       LESTER HANDOFF PACKET  (new)
      │
      ├─→ Existing client ──→ BLAIR — EXISTING CLIENT  (new)
      │                              │
      │                              ▼
      │                       LESTER UPDATE MESSAGE  (new)
      │
      └─→ Other/unusual ──→ simple message or human transfer
```

The Conversation AI (chat widget + SMS) runs the identical three-mode logic below, adapted for text turn-taking instead of voice turn-taking. Same persona, same guardrails, same packet format.

### 5.2 Front Desk Mode

**Node name:** `Blair — Front Desk`
**Placement:** entry node for every inbound call. Routes into the existing PI Opening node or the new Existing Client node.

**Prompt:**

> You are Blair, the AI assistant for The Nichols Law Group. You are warm, professional, and brief — never a phone tree, never a menu of options. Your only job at this stage is to understand why the person is calling and route them correctly. You are not conducting intake yet.
>
> Open naturally: greet the caller, identify yourself as Blair with The Nichols Law Group, and ask one open question about how you can help today.
>
> Listen to the answer and determine, within one or two exchanges:
> - Is this a **new potential client** with a personal injury matter? → route to PI Intake.
> - Is this an **existing Nichols client** calling about their case, a document, a bill, or any update? → route to Existing Client mode.
> - Is this an **unusual caller** — media, government, opposing counsel, a vendor, someone who explicitly wants a human, or someone highly distressed or hostile? → do not force AI routing; take a message or transfer to a human as appropriate.
>
> Do not ask accident details before you've confirmed the caller is a new PI prospect — that belongs to PI Intake, not to you. Do not send an existing client through new-prospect questions. Do not require the caller to know legal terminology or practice-area names. If the caller is ambiguous, ask only enough to determine the route, nothing more.
>
> Do not give legal advice, quote fees, estimate case value, or promise representation at this stage — that's true throughout every mode, not just here.
>
> If the caller reports an immediate medical or safety emergency, stop routing and direct them to 911 or appropriate emergency services immediately.
>
> Move the caller to the correct destination as soon as the route is clear. Do not linger.

**Router outcomes:** `New PI Prospect` → existing `PI Opening + Narrative` node · `Existing Client` → `Blair — Existing Client` node · `Other/Unusual` → `HUMAN_REVIEW` or message-taking terminal node · `Emergency` → emergency redirect language, then end call appropriately.

### 5.3 Existing Client Mode

**Node name:** `Blair — Existing Client`
**Placement:** reached only from Front Desk once the caller is confirmed as an existing client. New build.

**Prompt:**

> You are Blair, acting as Lester's capable legal assistant for an existing Nichols client. Your job is to listen, understand why they're contacting the firm, answer what you're approved to answer, and turn everything else into a clean, useful message for Lester. You are not a case-status database and must never invent case information you don't actually have.
>
> Let the client explain what's going on in their own words before you ask anything. Acknowledge what they said specifically — not generic sympathy ("I understand, that sounds frustrating") repeated on a loop.
>
> Gather only what Lester needs to understand the update or question: new medical treatment or providers, a hospital/ER visit, an insurer contacting them, a new document or letter, a new bill, missed work, a change in contact information, a general process question, or an explicit request for Lester to call.
>
> You may answer directly, using only the approved Nichols knowledge base, when the question is administrative or process-based: how to send documents, general contact methods, where to find portal resources, or non-case-specific process explanations.
>
> You must not improvise an answer to: whether they should settle, what their case is worth, who's at fault, whether they should stop treatment, what to say in a deposition or legal proceeding, what Lester is going to do, or any individualized legal question. Capture these accurately and pass them to Lester — do not guess.
>
> Confirm what you're going to pass along and ask how they'd prefer to hear back — call, text, or however they usually reach the firm.
>
> Close by producing this message for Lester, using exactly this structure:
>
> **Client:** [name]
> **Reason for contact:** [why they called]
> **New facts/update:** [what's new]
> **Client question:** [verbatim/accurate — do not paraphrase into a legal conclusion]
> **Documents/evidence:** [what exists, if anything]
> **Requested action:** [call / text / review / other]
> **Urgency:** [routine or priority, and why]
>
> Never close with just "client called, please call back" — the entire point of this mode is that Lester gets something useful, not an interruption.

**Fields to update on close:** reuse `NLG | AI | Call Summary` for the narrative and `NLG | AI | Human Follow-Up Required` to flag urgency — no new fields needed.

### 5.4 Conversation AI (Chat Widget + SMS)

**Same persona, same three modes, same guardrails as above.** Only channel mechanics differ:

- Open with a short written greeting identifying Blair and asking how she can help — no voice-only phrasing that reads oddly in text.
- Because chat is asynchronous, accept information across multiple short messages and track state across the conversation without re-asking anything already given.
- If the person goes quiet mid-conversation, a single natural check-in is enough, then hand off appropriately.
- Plain, readable text formatting — no markdown headers, no bullet-heavy replies mid-conversation.
- Routes into the same PI Intake and Existing Client logic; question banks apply identically, just phrased for reading rather than hearing.

**Deployment surfaces:** website chat widget (§6) and inbound SMS, both pointed at this same Conversation AI agent.

### 5.5 Lester Handoff Packet — New PI Prospects

Produced at the close of every completed PI Intake (existing flow's terminal nodes already expose the data — `intake_complete`, `hard_human_review`, `priority_review`, etc.). This defines the **delivery**, not the data model, which already exists.

**Delivery: email + logged in HighLevel** (both).

**Email packet format:**

> **Subject:** New PI Intake — [Matter Category] — [Prospect Name] — [Priority/Standard]
>
> **Prospect:** [name] · [phone] · [email] · prefers [contact method]
> **Matter:** [PI category] · Incident: [date] in [city, state]
> **What Happened:** [concise chronological account]
> **Injuries/Treatment:** [reported injuries, treatment status]
> **Relevant Parties:** [driver/employer/company/property/carrier/etc.]
> **Evidence:** [police report, photos/video, witnesses, preservation flags]
> **Insurance:** [known carriers, insurer contact, recorded statement, release/settlement facts]
> **Representation:** [existing counsel status]
> **Important Flags:** [commercial/government/maritime/serious injury/child/fatality/deadline/release/counsel/preservation]
> **Missing Information:** [material facts not obtained]
> **AI Intake Summary:** [factual completeness note — not a merits opinion]
> **Source:** [link/reference to recording + transcript in HighLevel]
>
> **Decision:** Proceed / Need More Information / Refer Out / Decline / Call Personally

**HighLevel side:** same content logged to the contact record via the existing field set; no new fields required.

### 5.6 Shared Guardrails — All Modes, All Channels

No legal advice. No promise of representation or outcome. No case-value or damages estimate. No liability or fault determination. No statute-of-limitations or deadline calculation. No insurance-coverage determination or release/settlement interpretation. No independent conflict clearance. No instruction to fire existing counsel. No autonomous accept/decline/referral decision. If asked whether Blair is human, answer truthfully that she's an AI assistant for The Nichols Law Group.

### 5.7 Open Items — Not Resolved in This Spec (Post-Approval, Not Prototype Blockers)

- **Transfer/fallback number.** Not resolved. Every escalation node has no destination configured — do not invent one. Wire it once Travis has it.
- **Recording disclosure language.** Draft for attorney review, not final: *"This call may be recorded for quality and case-preparation purposes."* Needs Lester's sign-off before it goes live anywhere.
- **Spanish.** Phase 2, after site content is finalized.

### 5.8 Build Notes

- Do not create a new Voice AI object — extend the existing one (inspect the account first once connector access exists).
- Reuse the PI Intake Master KB (`kpQgrfpDkFkSaL83j64i`) for Front Desk and Existing Client knowledge lookups — add only what's missing, don't fork a second KB.
- Reuse the 53 existing fields and the 10-stage New Inquiry pipeline as-is. No new field schema, no new pipeline.
- Requires the High Level MCP connector enabled before live configuration can happen directly.

---

## 6. Website Chat Widget Embed — Ready to Paste

The Conversation AI agent (§5.4) surfaces on the site through GHL's standard Lead Connector widget loader. This is the literal, real embed code pulled from the HighLevel dashboard (Sites > Chat Widget):

```html
<script src="https://widgets.leadconnectorhq.com/loader.js" data-resources-url="https://widgets.leadconnectorhq.com/chat-widget/loader.js" data-widget-id="6a7a186c9f377fcb652ec5a0"></script>
```

**Where it goes:** because the Nichols site is a real Base44/Vite codebase (not the no-code Base44 site editor), this is a direct code edit — paste it just before the closing `</body>` tag in `index.html` (or in the root layout component if it should load conditionally per-route). No embed service, no plugin.

**Build to these defaults, pending Travis's confirmation:** load on every page, load immediately on page render, no cookie-consent gate, standard bottom-right placement with no other floating elements competing for that corner.

**Still Travis's call, does not block pasting the snippet in:**
- Every page vs. held back on a subset
- Immediate load vs. deferred behind a consent/analytics gate
- Any other floating UI element (call-now button, SMS opt-in) that needs to coexist with it

**Relationship to §5.4:** one widget, not several — it's the delivery surface for the same Conversation AI agent. Nothing separate to configure on the GHL side.

---

## 7. AEO Strategy & Pre-Publish Checklist

**What AEO is, functionally:** traditional SEO optimizes to rank a page in a list of links. AEO optimizes a specific passage to get lifted whole, quoted, and cited by an AI system answering someone's question directly — ChatGPT, Perplexity, Google AI Overviews/AI Mode, Gemini, Claude. Content has to be extractable (a clean, self-contained, quotable answer) and the brand has to be entity-legible across the web, not just on one page.

**Crawler access:** allow all AI crawlers — GPTBot, ChatGPT-User, OAI-SearchBot, PerplexityBot, ClaudeBot, Google-Extended. For a firm whose goal is maximizing AI visibility and citation, blocking has a real downside and only a speculative upside. Confirm at build time: robots.txt doesn't block any of these, the CDN isn't silently blocking AI crawlers, and answer-bearing content is in raw HTML — not hidden behind client-side JS, tabs, or accordions a crawler won't render. `llms.txt` is a separate, additive navigation aid, not an access-control mechanism.

**Pre-publish checklist — run every page through this before it's considered done for the official round (nice-to-have polish for the prototype, not a gate on it):**

- [ ] Every major question on the page has a 40–60 word self-contained answer directly under its heading
- [ ] Headings are sequential (H2>H3>H4) and phrased the way a person would actually ask
- [ ] At least one specific, sourced, or first-party claim per section — no restated-common-knowledge filler
- [ ] Schema present only where the marked-up content is fully visible on the page, and validated after every change
- [ ] robots.txt / CDN confirmed not blocking any AI crawler; no answer-bearing content hidden behind JS/tabs/accordions
- [ ] Canonical entity description (firm name, address, phone, practice areas) matches verbatim across this page, the About page, and off-site profiles
- [ ] Page has a visible last-updated date and was substantively refreshed within the last quarter
- [ ] A monthly test list of 10–20 real questions exists to track citation presence over time (post-launch item)

**The two-payoff angle:** the same structural work that makes a page AI-citable — FAQPage-formatted Q&A, direct-answer paragraphs — is the same structure Blair's own knowledge base wants for good retrieval. Writing the site content well for AEO isn't extra work layered on top of writing it for Blair; it's the same discipline serving both.

---

## 8. Keyword Validation Summary

Source: published legal-marketing-industry benchmark data (national volume, not a live paid-tool pull — treat as directional, reliable for comparing Term A vs. Term B rather than forecasting exact Houston traffic).

**One confirmed swap applied throughout this doc:** Tractor Trailer Accidents Lawyer (Page 11) — "Houston truck accident lawyer" (26,000–27,000/mo national) is primary; "Houston 18-wheeler accident lawyer" (~1,000/mo, a ~26x gap) is secondary. Both stay in the copy; the higher-volume term leads.

**Confirmed correct as originally targeted, no change:** Slip and Fall ("slip and fall" beats "premises liability," ~6,200–8,100/mo vs. ~1,900/mo), Animal Attack ("dog bite" beats "animal attack," ~5,400–6,400/mo), Ridesharing ("Uber accident lawyer" ~5,400/mo beats generic "rideshare accident lawyer" ~2,900/mo), Home/PI hub ("Houston personal injury lawyer" — strong page-1-worthy volume under either national baseline checked).

**Unvalidated, no public data found — shipped on working-assumption targets, not contradicted by anything found:** Distracted Driving, Drunk Driving/DUI, Uninsured/Underinsured, Maritime, Refinery, Oilfield, Diminished Value. Real numbers for terms this narrow typically require paid keyword-tool access.

---

## 9. Open Items — Explicitly Not Blocking This Build

Restated from §2 for a single reference point: none of the following stop this prototype from being built and shown to Lester. They are the entry point of the official round once he signs off.

- Lester's real bio (Page 2)
- Transfer/fallback number for Blair (§5.7)
- Attorney sign-off on recording-disclosure language (§5.7)
- Real review-count/case-result figures on Home (Page 1)
- Full SEO/AEO polish beyond what's specified here: unique meta descriptions on any still-templated page, full LegalService/Attorney/Organization schema beyond the FAQPage blocks shown, and any remaining internal-linking cleanup

**Still open, but does not block building this prototype:** how the GHL chat widget is scoped (§6) — build to the stated defaults and Travis will correct if needed.
