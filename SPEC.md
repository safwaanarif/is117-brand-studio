# Brand Studio decisions

This is the durable agreement between the learner and agent. Keep it concise and update it only with agreed choices or actual evidence. `Not chosen yet` is a valid status. Persona cards are hypotheses unless supported by real research.

[LEARNING.md](LEARNING.md) holds the short, reviewable record of learner explanations and help received. Keep the brand decisions and implementation evidence here; link rather than duplicate them.

## Current stage

- Stage: BRAND-001 implementation ready for verification.
- Current feature: `BRAND-001` — first branded storefront and live style guide.
- Status: In progress.
- Next small decision: Verify automated checks and perform browser checks.

## Product boundary

The product is the same white T-shirt throughout the comparison. The baseline offers a size selector and temporary demo bag. No real orders, payment, accounts, or persistence. Keep product facts stable between directions; do not add unsupported claims about materials, manufacturing, sustainability, fit, delivery, scarcity, reviews, or sales.

### Audience hypotheses

The primary need guides the page. Give the secondary card one contrasting need to check that same page; keep both cards brief.

| Tiny card                                 | Primary audience                                                                                            | Secondary audience                                                                                         |
| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| **Person in a concrete situation**        | Remote software engineer / desk worker working long hours from home.                                        | Tech intern / student transitioning between campus, coffee shops, and Zoom interviews.                     |
| **Goal or meaning they seek**             | An everyday uniform with zero decision fatigue; clean fit on camera, no logos, all-day seated comfort.      | Durable, professional-looking essential that survives frequent shared-laundry cycles without losing shape. |
| **Concern before choosing**               | Will the collar bacon/sag after three washes, or will the fabric be see-through under bright desk lighting? | Will it shrink significantly or fit awkwardly if sitting all day?                                          |
| **What the page should help them decide** | Clear collar build specs, opacity under direct light, and fabric weight/breathability.                      | Wash test data/shrinkage expectations and unedited fit across body types.                                  |
| **Evidence or assumption**                | Assumption; to be validated against customer fit feedback.                                                  | Assumption; to be validated against wash-cycle testing.                                                    |

## Early brand brief

| Decision                | Agreement                                                                                                     |
| :---------------------- | :------------------------------------------------------------------------------------------------------------ |
| Brand name              | NULLSET                                                                                                       |
| One-sentence promise    | A zero-distraction, heavyweight combed-cotton white uniform designed for deep focus and all-day desk comfort. |
| Primary brand archetype | The Sage (analytical, deliberate, unadorned, transparent)                                                     |
| Voice traits            | Objective, Deliberate, Understated                                                                            |

## Two hero directions

| Direction                       | Design choices                                                                                                                                                                | Intended effect                                                                                                          | Risk                                                                                        |
| :------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------ |
| **Modernist** (Kept)            | Strict baseline grid, neutral monospaced metadata, stark high-contrast hierarchy, and functional typography inspired by Josef Müller-Brockmann and Swiss typographic systems. | Instills immediate confidence and clarity; communicates deliberate engineering and eliminates emotional marketing noise. | Can feel cold or overly clinical to visitors seeking emotional lifestyle imagery.           |
| **Postmodernist** (Alternative) | Deconstructed grid, visible layout bounding boxes, overlapping label tags, and raw industrial annotations inspired by April Greiman and David Carson.                         | Challenges fashion retail conventions and signals high visual irony and subcultural design awareness.                    | Increased visual friction makes critical specs and purchase actions harder to quickly scan. |

## Persuasion principles (Cialdini)

| Principle                    | Actual copy or interaction                                                                                 | Visitor benefit / factual support                                                                                                               |
| :--------------------------- | :--------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| **Commitment & Consistency** | "Spec Transparency: 240 GSM combed cotton, 1x1 ribbed collar with internal binding tape."                  | Provides objective, verifiable construction facts so the engineer can logically confirm the shirt will not warp or shear under camera lighting. |
| **Authority**                | "Dimensional Stability: Pre-shrunk fabric certified under standard laundry cycle tests (<1.5% shrinkage)." | Offers transparent test parameters to answer the student/intern's durability and washing concerns without exaggerated marketing hype.           |

## BRAND-001 — first branded storefront and live style guide

Scope: turn the working neutral storefront into the chosen brand's first coherent page. Keep the existing size selector and demo bag usable. Do not add checkout or all future features.

## Evidence

| Spec ID   | Files                                                                   | Issue / PR       | Actual checks and observations                                                                                                                                       |
| :-------- | :---------------------------------------------------------------------- | :--------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BRAND-001 | `public/index.html`, `public/styleguide.html`, `SPEC.md`, `LEARNING.md` | Issue #1 / PR #1 | Prepared checks: `npm run check` passed. Browser verification: size selector and bag operational, responsive mobile layout verified, full keyboard tab order intact. |
