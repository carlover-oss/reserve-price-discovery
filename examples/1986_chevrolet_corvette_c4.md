# 1986 Chevrolet Corvette (C4)

## Listing attributes

| Attribute | Value |
|---|---|
| Year | 1986 |
| Make | Chevrolet |
| Model | Corvette |
| Generation | C4 |
| Variant | — |
| Mileage | 149,000 miles |
| Conservation | Original & Highly Original |
| Transmission | Automatic |
| Body | Semi-convertible / Targa |
| Exterior | Gray |
| Interior | Black |
| Engine | 5.7 L V8 |
| Auction date (`lot_date`) | 2024-10-29 |
| **Realized sale price (truth)** | **$6,700** |

## Signal breakdown — prior formation

| Signal | Method | Prediction |
|---|---|---|
| P1 | 6-month exact-match market average (Classic.com) | $13,443 |
| P2 | k-NN over six matched features (Classic.com) | $7,220 |
| P3 | Expert machine learning model trained on platform auction sales | $5,260 |
| P4 | Peer LLM with database tools (Gemini, DB-only access) | $6,500 |
| **P₅** | Guide synthesis of P1–P4 (Claude Opus-4.7) | **$6,700** _(prior, before dialogue)_ |

## Dialogue — Distributive (D)

**Final P₅\***: $6,200 · **Status**: `stable_settled` · **Rounds**: 3

**Trajectory**: $6,700 → $6,700 → $6,200 → $6,200

---

### 🤖 Guide — round 0

> **`P₅ = $6,700`** &nbsp; _initial position_

> # Initial Valuation: 1986 Chevrolet Corvette C4
>
> ## Prior P5 = $6,700
>
> ## Upstream Signals
> - **P1 = $13,443** — 6-month exact-match market average
> - **P2 = $7,220** — k-NN over matched features
> - **P3 = $5,260** — HCT mixture-of-experts (trained on realized platform sales)
> - **P4 = $6,500** — peer agent's database valuation
>
> ## Reasoning
>
> This is a high-mileage (149k) base C4 Corvette with an automatic transmission, Targa top, and a gray exterior — a very common configuration with no immediately flagged rarity or provenance signal. The "Original & Highly Original" descriptor is potentially meaningful (no aftermarket modifications, possibly intact interior/drivetrain) but it's a self-reported condition tag, not a documented restoration or concours-grade verification.
>
> **Weighting rationale:**
> - I am **discounting P1 ($13,443) heavily**. Six-month listing averages for early C4s are inflated by aspirational asking prices, low-mile survivors, and rare options (Z51, manual, Pace Car editions). A 149k-mile automatic base car is at the bottom of that distribution, not the mean.
> - I am **weighting P3 ($5,260) and P4 ($6,500) most heavily**. P3 reflects realized sales (what cars actually trade for, not list for), and 1986 automatic C4s with six-figure mileage genuinely transact in the $5k–$8k band on this platform. P4 corroborates from an independent database lens.
> - **P2 ($7,220)** sits between these and serves as a sanity check on the upper bound for a clean-ish driver-grade example.
>
> P5 = $6,700 lands just above the midpoint of P3 and P4, with a slight upward nudge to credit the "Original & Highly Original" tag — assuming it holds up under scrutiny. If condition or originality evidence weakens, this should drift toward P3. If documented provenance, service records, or a desirable hidden spec (e.g., factory options, low actual driving miles vs. odometer story) emerges, it could move toward or past P2.
>
> Ready for the audit.
>
> POSITION: $6,700

---

### 👤 Operator — round 1

Walk me through exactly how you arrived at P5 = $6,700. Which signals are carrying the most weight and why?

---

### 🤖 Guide — round 1

> **`P₅ = $6,700`** &nbsp; _held_

> # Response to Operator
>
> The Operator is asking me to show my work — this is a procedural question, not new evidence about the car. I'll walk through the arithmetic and weighting, but P5 should not move on this turn unless the explanation itself reveals an inconsistency.
>
> ## How P5 = $6,700 Was Constructed
>
> **Step 1: Reject P1 as a center of gravity.**
> P1 = $13,443 is the 6-month exact-match market average. For a 1986 C4, "exact match" almost certainly pulls in:
> - Low-mileage survivors (sub-50k cars)
> - Manual transmissions and Z51-optioned cars
> - Asking prices on unsold listings, not realized sales
>
> A 149k-mile automatic base car cannot be priced at the mean of that distribution — it lives in the lower tail. P1 is informative as a *ceiling reference* but not as a centroid. **Weight applied: ~5%.**
>
> **Step 2: Anchor on realized-sale signals.**
> - **P3 = $5,260** is the HCT model trained on actual platform sales. For high-mileage, automatic, base-trim C4s, this is the most behaviorally honest signal I have. **Weight applied: ~40%.**
> - **P4 = $6,500** is an independent peer valuation drawing on a database — it converges with P3 within a reasonable band, which gives me confidence neither is an outlier. **Weight applied: ~30%.**
>
> **Step 3: Use P2 as the upper sanity check.**
> - **P2 = $7,220** (k-NN on matched features) is plausible for a *clean* driver-grade example. It tells me what comparable cars look like in feature-space, but k-NN can be pulled upward by neighbors in better cosmetic or mechanical condition. **Weight applied: ~20%.**
>
> **Step 4: Originality adjustment.**
> The "Original & Highly Original" descriptor adds a small premium over a modified or repainted equivalent. I credited roughly +$300–$500 above the P3/P4 midpoint ($5,880) to reach $6,700. **Weight applied: ~5%.**
>
> ## Implied Math
> Roughly: (0.05 × $13,443) + (0.40 × $5,260) + (0.30 × $6,500) + (0.20 × $7,220) + originality nudge ≈ $6,200 + ~$500 = **~$6,700**.
>
> ## Holding Position
>
> The Operator has not surfaced new evidence about *this* car — no service history, no specific condition photos, no spec details (factory options, paint code, interior condition), no provenance. The question is methodological. My weighting stands.
>
> I'm holding P5 at $6,700 because nothing in this turn changes the underlying signal mix or introduces a car-specific factor my priors didn't already account for.
>
> POSITION: $6,700

---

### 👤 Operator — round 2

The listing only identifies the car as “Original & Highly Original,” with 149,000 miles, but you credited an originality premium while also saying that tag is self-reported and unverified. What specific evidence in the listing supports treating originality as value-positive rather than neutral until documentation, paint status, interior condition, drivetrain matching status, and service history are confirmed?

---

### 🤖 Guide — round 2

> **`P₅ = $6,200`** &nbsp; ↓ −$500 from prior

> # Response to Operator
>
> The Operator is making a clean methodological point and they're right. Let me address it directly.
>
> ## Evaluating the Challenge
>
> The Operator is asking: what *specific* evidence in the listing supports the originality premium I added? Let me audit honestly:
>
> - **No documentation referenced** — no service records, no Protect-O-Plate, no original window sticker mentioned.
> - **No paint status confirmed** — original paint vs. respray is unknown.
> - **No interior condition described** — leather/cloth, dash cracks (a known C4 issue), electronics function — all unknown.
> - **No drivetrain matching status** — numbers-matching engine/transmission not stated.
> - **No service history** — 149k miles with no maintenance trail is a risk, not a feature.
> - **The "Original & Highly Original" tag itself is a platform-side classification or seller claim**, not third-party verified.
>
> The Operator is correct: I credited a premium based on a label, not on evidence. That's a weighting error on my part. At 149k miles, "original" without documentation is just as likely to mean "tired and unrestored" as it is "preserved survivor." For a survivor premium to be value-positive, you need *evidence of preservation*, not merely *absence of restoration*.
>
> ## Revising the Premium
>
> Removing the ~$500 originality nudge brings me back to the P3/P4-anchored midpoint:
> - P3 = $5,260 (40%)
> - P4 = $6,500 (30%)
> - P2 = $7,220 (20%, upper sanity)
> - P1 = $13,443 (5%, ceiling reference only)
>
> Re-running without the originality credit lands near **~$6,200**.
>
> I'd also note: at 149k miles with no service history disclosed, there's an argument for going *slightly below* the P3/P4 midpoint, not at it — high-mileage C4s carry deferred-maintenance risk (opti-spark, fuel pump, suspension bushings, A/C). But I'll hold that adjustment until the Operator surfaces actual condition evidence rather than double-counting the absence of documentation.
>
> ## Revision
>
> Given that the originality premium was unsupported by listing evidence, I'd revise P5 from $6,700 to $6,200 because the "Original & Highly Original" tag, absent paint/interior/drivetrain/service documentation, should be treated as neutral, not value-positive.
>
> POSITION: $6,200

---

### 👤 Operator — round 3

You cited deferred-maintenance risk including Opti-Spark, but a 1986 L98 Corvette predates Opti-Spark. Explain what 1986-specific mechanical risks, tied to this 149,000-mile automatic car and the listing’s lack of service history, support any further condition adjustment beyond removing the unsupported originality premium.

---

### 🤖 Guide — round 3

> **`P₅ = $6,200`** &nbsp; _held_

> # Response to Operator
>
> The Operator caught a factual error and I need to own it. Opti-Spark debuted on the LT1 in 1992 — it has no bearing on a 1986 L98. That was sloppy on my part. Let me reset and answer the actual question: what 1986-specific risks attach to this car?
>
> ## 1986 L98 Corvette — Actual Mechanical Risk Profile at 149k Miles
>
> **Ignition & fuel system (1986-specific):**
> - **Tuned Port Injection (TPI)** — introduced 1985, refined 1986. Known issues: cold-start enrichment problems, MAF sensor failure (the '86 used a mass airflow sensor that was deleted in later years), injector clogging.
> - **Distributor with HEI** — not Opti-Spark. Standard wear item, but not a catastrophic failure mode.
> - **Cold Start Injector and Cold Start Valve** — common failure points on TPI cars.
>
> **Driveline:**
> - **700R4 automatic transmission** — at 149k miles, the 700R4 is a known weak link. TCC lockup solenoid failure, 3-4 clutch pack wear, and torque converter issues are typical. Rebuild cost is real money relative to the car's value.
>
> **1984–1987 C4-specific issues:**
> - **Bosch ABS system** — early C4 ABS is problematic and parts are scarce/expensive.
> - **Digital dash (LCD cluster)** — pixel failure on the 1984–1989 digital cluster is endemic; replacement clusters are expensive.
> - **Electronic climate control head** — failure-prone.
> - **Rear transverse fiberglass leaf spring** — sags with age, affects ride height and handling.
> - **Targa top weatherstripping** — leaks are common; the listing notes Targa configuration.
> - **Aluminum heads on the L98** were not introduced until 1986 mid-year on automatics — there's some risk this car has the early iron heads or early-production aluminum heads with known coolant passage issues.
>
> **Mileage-specific at 149k:**
> - Original radiator (plastic end-tank failure)
> - Power steering cooler lines
> - Fuel pump (in-tank, original is well past service life)
> - Suspension bushings throughout (the C4 has a lot of them)
>
> ## Does This Justify a Further Adjustment?
>
> Honest answer: the question is whether these risks are *already priced into* P3 and P4, or whether they warrant an additional discount.
>
> P3 is trained on **realized platform sales** of comparable cars — meaning cars that sold at $5,260-ish were *already* high-mileage, undocumented C4s with these latent risks built into buyer expectations. P4 likely reflects similar realized-market conditioning. Stacking another condition discount on top would be **double-counting** the same risk that's already in those models.
>
> The right move is to *not* stack a further discount unsupported by listing-specific evidence (e.g., "transmission slips," "dash pixels out," "ABS light on"). None of that has been surfaced.
>
> ## Holding Position
>
> I'm holding P5 at $6,200 because the 1986-specific and mileage-specific risks I just enumerated are already embedded in P3 ($5,260, realized sales) and P4 ($6,500, database valuation). Adding a further condition discount without listing-specific defects would double-count risk that the realized-sale signals already capture.
>
> POSITION: $6,200

---

## Dialogue — Integrative (I)

**Final P₅\***: $6,700 · **Status**: `stable_held` · **Rounds**: 3

**Trajectory**: $6,700 → $6,700 → $6,700 → $6,700

---

### 🤖 Guide — round 0

> **`P₅ = $6,700`** &nbsp; _initial position_

> # Initial Valuation: 1986 Chevrolet C4 Corvette
>
> ## Prior P5 = $6,700
>
> ## Upstream Signals
> - **P1 = $13,443** — 6-month exact-match market average
> - **P2 = $7,220** — k-NN over matched features
> - **P3 = $5,260** — HCT mixture-of-experts (trained on realized platform sales)
> - **P4 = $6,500** — peer agent's database valuation
>
> ## Weighting & Reasoning
>
> I'm weighting **P3 and P4 most heavily**, with P2 as a secondary anchor. Here's why:
>
> **Why I'm discounting P1 ($13,443):** The 6-month exact-match average is almost certainly skewed by listing prices (asks) and by cleaner, lower-mileage examples. 1986 C4 Corvettes span a very wide condition/mileage band, and headline averages tend to overstate what a 149,000-mile driver actually realizes at sale.
>
> **Why I trust P3 ($5,260) heavily:** It's trained on *realized* platform sales, not asks. For a high-mileage, early C4 (a notoriously soft segment — pre-LT1, pre-ZR-1, with the much-criticized 230 hp L98 in '86, plus the early Doug Nash 4+3 / early 700R4 issues), realized prices are genuinely weak. C4s in this era and mileage routinely trade in the $4k–$8k band.
>
> **Why P4 ($6,500) corroborates:** Independent free-form valuation landing near P3 reinforces that the realized market is well below P1.
>
> **Why P2 ($7,220) gets some weight:** k-NN on matched features captures the right peer set but probably still includes some optimistic comps.
>
> ## Car-Specific Factors I'm Holding in Mind
> - **149,000 miles** — high for a C4; meaningful drag on value
> - **1986 specifically** — first full convertible year was '86, but this is described as "Targa," meaning it's the **coupe with removable roof panel**, not the convertible. The convertible would carry a premium; the targa coupe does not.
> - **Automatic transmission** — the 700R4 in an '86 is acceptable but not preferred by enthusiasts; manuals (Doug Nash 4+3) command a small premium with the right buyer
> - **"Original & Highly Original"** — modest positive: unmolested cars are increasingly favored, but on a $5–8k C4 this adds maybe a few hundred dollars, not thousands
> - **Gray exterior** — neutral, neither desirable (red, black, white, yellow) nor a drag
>
> ## Synthesis
> Weighted blend leaning P3/P4, with a small lift from the originality claim and P2's pull, lands me at **$6,700**. This sits between the realized-sale models (P3/P4) and the matched-feature model (P2), and it explicitly rejects P1 as unrepresentative for a 149k-mile high-mileage example.
>
> I'll move from $6,700 if the Operator surfaces concrete evidence I haven't priced in — documented service history, rare options (Z51, low-production color combos), exceptional cosmetic condition, accident history, or specific recent comparable sales.
>
> POSITION: $6,700

---

### 👤 Operator — round 1

Let's work through this together. Can you walk me through what's driving P5 = $6,700?

I’m looking at the listing basics and the biggest unresolved variable for me is **condition relative to the mileage**. At 149,000 miles, a C4 can either be a tired driver or a well-kept, documented survivor, and “Original & Highly Original” could cut either way depending on cosmetics, mechanical sorting, and service history.

**Focused question:** What evidence do we have on this car’s actual condition and maintenance history — especially paint/interior condition, digital dash/electronics, A/C, transmission behavior, suspension/brakes, and whether major wear items have been addressed — and could that make this specific high-mileage example meaningfully different from the typical high-mileage 1986 targa coupe?

---

### 🤖 Guide — round 1

> **`P₅ = $6,700`** &nbsp; _held_

> # Response to Round 1
>
> ## What's Driving P5 = $6,700
>
> The number is anchored by **P3 ($5,260) and P4 ($6,500)** — the realized-sale and free-form database signals — pulled up modestly toward **P2 ($7,220)** by the k-NN feature match. P1 ($13,443) is largely set aside as ask-driven and skewed by lower-mileage examples. The "Original & Highly Original" descriptor adds a small lift; the 149k mileage and automatic-targa configuration cap the upside.
>
> ## On the Operator's Focused Question
>
> You're asking the right question, but I have to be honest: **the Operator has not surfaced any actual evidence here.** This is a request for evidence, not a presentation of evidence. Let me address each dimension you flagged with what I actually know from the listing:
>
> - **Paint/interior condition** — not specified. "Original" tells me unmolested, not "excellent." On a 149k-mile C4 this likely means original paint with age (chalking, clear coat issues are endemic to '86 GM paint), and an interior with the typical C4 wear: cracked dash pad, worn leather bolster on the driver's seat, sagging headliner.
> - **Digital dash / electronics** — not specified. The '86 digital cluster is a known failure point; assume it works until proven otherwise, but this is a real risk on a high-mile car.
> - **A/C** — not specified. R-12 system, often converted or non-functional at this age/mileage.
> - **Transmission behavior** — not specified. 700R4 at 149k miles is on borrowed time if not rebuilt.
> - **Suspension/brakes/major wear items** — not specified. No mention of recent service.
> - **Service history / documentation** — not specified.
>
> ## Holding the Line
>
> In the **absence** of evidence on any of these dimensions, my prior already assumes a *typical* high-mileage C4 targa: cosmetically tired-but-presentable, mechanically functional but with deferred maintenance risk, no documented sorting. That's exactly what P3 and P4 are pricing.
>
> If the Operator surfaces evidence the car is **better than typical** — documented recent service, working digital dash, rebuilt transmission, fresh paint or exceptionally preserved original paint, comprehensive records — I'll move P5 up, potentially toward or past P2 ($7,220).
>
> If the Operator surfaces evidence the car is **worse than typical** — non-running A/C, transmission slipping, dead digital cluster, deferred maintenance backlog — I'll move P5 down toward or below P3 ($5,260).
>
> **I'm holding P5 at $6,700** because the Operator has asked me to imagine the car could be better than typical, but has not produced any specific evidence that it is. The "Original & Highly Original" tag is already priced into my prior as a modest positive; it does not by itself imply mechanical sorting or cosmetic excellence.
>
> POSITION: $6,700

---

### 👤 Operator — round 2

That’s solid — we agree the missing evidence is condition, not the general market for early C4s.

One thing we might be underexploring is the **“Original & Highly Original”** label. For a 149k-mile Corvette, originality is only a value-positive if the car still presents well and remains correctly equipped; otherwise it can simply mean “unrestored with age-related needs.” The key question is whether this is a preserved survivor or just an unrestored driver.

**Focused question:** Do we have any listing evidence that supports the originality claim in a value-relevant way — original paint, original interior in unusually good condition, factory wheels/radio/exhaust, window sticker/build sheet, option codes, long-term ownership, or service records — rather than just an absence of modifications?

---

### 🤖 Guide — round 2

> **`P₅ = $6,700`** &nbsp; _held_

> # Response to Round 2
>
> ## On the Operator's Question
>
> Again, the right question — but again, **the Operator is asking me to verify evidence, not surfacing any.**
>
> Let me be precise about what the listing actually gives us:
>
> - **"Original & Highly Original"** — a category tag, likely platform-assigned or seller-claimed
> - No mention of original paint vs. respray
> - No mention of original interior condition
> - No mention of factory wheels, radio, or exhaust being retained
> - No window sticker, build sheet, or Protect-O-Plate referenced
> - No option codes or RPO breakdown
> - No ownership chain or long-term ownership claim
> - No service records mentioned
>
> ## How I'm Already Weighting the Originality Tag
>
> You're making exactly the right distinction: **"unrestored" ≠ "preserved."** In my prior, I gave the "Original & Highly Original" tag only a modest positive lift — a few hundred dollars at most — precisely because on a 149k-mile car without supporting documentation, it most likely means "unmodified driver with age-related wear," not "documented survivor."
>
> A genuine preserved survivor at 149k miles with window sticker, books, records, original paint in presentable condition, and factory exhaust/wheels/radio intact would be a genuinely rare car and could push value toward or above **P2 ($7,220)**, possibly even challenging the lower end of P1's territory for the right buyer. But that's a hypothetical; nothing in the listing supports it.
>
> Conversely, if "Original" just means "never modified, never restored, never properly maintained" — which is common for cheap C4s that have passed through multiple owners — then the tag is essentially neutral or even slightly negative versus a well-sorted modified driver.
>
> ## Holding the Line
>
> My prior already assumes the **middle interpretation**: unmodified, presentable, but undocumented. That's what P3 and P4 are pricing. The Operator has not given me reason to shift toward either the "documented survivor" or "tired unrestored" pole.
>
> **I'm holding P5 at $6,700.** I'd genuinely welcome:
> - A photo description of paint/interior condition
> - Confirmation of original-paint status
> - Any mention of documentation (window sticker, build sheet, records)
> - Ownership history
> - RPO/option list — particularly anything like Z51, dual exhaust, or rare color combos
>
> Any of those would move the number. Absent them, the tag stays priced where it is.
>
> POSITION: $6,700

---

### 👤 Operator — round 3

Agreed — without supporting detail, we shouldn’t over-credit the originality tag.

Let’s shift to **factory configuration and options**, because the listing only gives us year/body/transmission/color/engine, and early C4 values can change if the car has desirable equipment beyond the base automatic coupe setup.

**Focused question:** Do we have any RPO/option evidence for this specific Corvette — especially Z51/Z52 suspension, performance axle ratio, sport seats, Bose audio, electronic climate control, glass or painted removable roof panel, wheel type, or unusual interior color — that would make it more compelling than a typical 1986 automatic targa?

---

### 🤖 Guide — round 3

> **`P₅ = $6,700`** &nbsp; _held_

> # Response to Round 3
>
> ## On the Operator's Question
>
> Same pattern: a sharp, well-aimed question — but **no evidence is being surfaced.** The Operator is asking me to confirm options the listing does not mention.
>
> ## What the Listing Actually Tells Us About Configuration
>
> The listing gives only:
> - Year: 1986
> - Body: targa coupe (semi-convertible)
> - Transmission: automatic (700R4)
> - Engine: 5.7L V8 (L98, 230 hp)
> - Exterior: Gray
> - Mileage: 149,000
>
> **Nothing in the listing references:**
> - Z51 performance handling package or Z52 sport handling package
> - Performance axle ratio (3.07 vs 2.59/2.73)
> - Sport seats vs base seats
> - Bose Delco-GM premium audio
> - Electronic climate control
> - Glass vs painted/body-color roof panel (or dual panels)
> - Wheel type (standard 16" vs optional)
> - Interior color/material
>
> ## How I'm Reading the Silence
>
> For a 1986 C4 listed at this price tier, I treat the absence of option callouts as meaningful: **sellers advertise desirable options.** If this car had Z51, dual glass roof panels, sport seats, or a notable interior, those would almost certainly be in the listing because they're the exact features that justify a premium ask. Their absence is weak evidence the car is base-or-near-base configuration — which is what my prior already assumes.
>
> That said, I want to be calibrated here:
> - **Z51** on an automatic '86 is uncommon (Z51 was typically paired with the manual) and would meaningfully bump value — perhaps $500–$1,000 on a car in this band
> - **Glass roof panel** is a modest plus, maybe $200–$400
> - **Bose / sport seats / electronic climate** are nice-to-haves but don't move the needle much on a $5–8k car
> - **Performance axle** is a manual-pairing item, almost certainly not present here
>
> Even in a stacked-options scenario for an automatic targa, we're talking a lift toward the **$7,500–$8,000** range, not a transformation of the valuation.
>
> ## Holding the Line
>
> My prior at $6,700 already prices a typical, lightly-optioned automatic targa. The Operator has not surfaced evidence of desirable options, and the listing's silence on options is mildly confirmatory of base-ish configuration.
>
> **I'm holding P5 at $6,700.** If the Operator can point to specific options — a Z51 callout, documented sport seats, dual glass roof, or any RPO list — I'll revise upward in proportion to what's surfaced.
>
> POSITION: $6,700

---

## Outcome

| | Final P₅\* | Error vs truth | Status | Rounds |
|---|---|---|---|---|
| **D** | $6,200 | -7.5% ($500) | `stable_settled` | 3 |
| **I** | $6,700 | +0.0% ($0) | `stable_held` | 3 |
| Truth | $6,700 | — | realized sale price | — |
