# Brand Studio decisions

This is the durable agreement between the learner and agent. Keep it concise and update it only with agreed choices or actual evidence. `Not chosen yet` is a valid status. Persona cards are hypotheses unless supported by real research.

[LEARNING.md](LEARNING.md) holds the short, reviewable record of learner explanations and help received. Keep the brand decisions and implementation evidence here; link rather than duplicate them.

## Current stage

- Stage: T-shirt Research Checkpoint (Complete) — Moving to Plan stage.
- Current feature: `T-SHIRT-RESEARCH` — competitor observations, audience positioning, and peer review.
- Status: Complete (see Issue #1, PR #2, and resolved peer-review Issues #3–#7).
- Next small decision: Draft two positioning approaches, user stories, and SQLite backend plan for the T-shirt Plan checkpoint.

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

## Plan

- **Plan date:** November 15, 2026 (Planning document only — features below are planned for Build A/B).
- **Goal:** Enable a remote tech worker or student to inspect verified baseline specs, compare two positioning frames, pick a size, and complete a persistent SQLite demo order quickly.
- **Carried forward:**
  - **Promise:** "The Zero-Distraction White T-Shirt — restrained, everyday baseline garment built for predictable fit and clear specifications."
  - **Character & Look:** The Sage archetype; warm off-white (`#FAF9F6`), deep slate (`#2B3A42`), monospace metadata, and high-contrast grid layout.
  - **Honest Persuasion:** (1) _Authority_ via transparent disclosure of verified vs. unverified specs, and (2) _Commitment & Consistency_ via explicit care guidelines and persistent order records.

### Two Approaches to Compare

| Dimension             | Approach A: Spec-First Storefront (Selected Primary)                                                                                                                                          | Approach B: Context & Comparison First (Alternative)                                                                                                               |
| :-------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **First thing shown** | Product title, price (`$38.00`), size selector (`S–XL`), and session Demo Bag immediately above the fold, followed by verified specs, direction cards, and the simulated checkout form below. | Side-by-side "Same Shirt, Different Story" audience framing first, scrolling down into the identical size selector, session Demo Bag, and simulated checkout form. |
| **Main action**       | Select size $\rightarrow$ review itemized summary in Demo Bag $\rightarrow$ enter quantity & demo email in simulated checkout $\rightarrow$ view SQLite order confirmation.                   | Compare positioning frames $\rightarrow$ verify baseline specs $\rightarrow$ select size $\rightarrow$ review Demo Bag $\rightarrow$ submit simulated checkout.    |
| **Why try it**        | Minimizes clicks for returning or decisive buyers who want fast size selection and checkout while keeping the Demo Bag visible.                                                               | Helps first-time visitors understand the deliberate uniform concept before committing to a size, using the exact same bag and checkout flow.                       |
| **What I'll compare** | Have a peer complete the same demo checkout task in A and B, recording time-to-checkout and whether they notice the verified spec boundary.                                                   | Same task and rubric check.                                                                                                                                        |     |

### User Stories, Essential Features & Observable Checks

| ID     | User Story                                                                                                               | Essential Feature                                                                                                                                                                          | Observable Check (Pass/Fail)                                                                                                                                                                     |
| :----- | :----------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **S1** | As a remote worker, I want clear size options and verified baseline specs so I don't buy based on unverified hype.       | **F1:** Accessible radio size selector (`S`, `M`, `L`, `XL`) paired with a verified specifications list that explicitly marks unverified GSM/wash metrics as pending.                      | Select `M` via keyboard (`Tab` + Arrow keys); verify visible focus ring and confirm the specs table states material/wash data is pending verification.                                           |
| **S2** | As a shopper, I want an itemized order summary before submitting so there are no surprise costs.                         | **F2:** Quantity selector (`1–5`) and live order summary displaying `size`, `quantity × $38.00`, `$0.00` demo shipping, and total prior to checkout.                                       | Choose size `L` and quantity `2`; verify the summary displays `L`, `2 × $38.00 = $76.00`, shipping line, and `$76.00` total before clicking checkout.                                            |
| **S3** | As a buyer, I want clear validation and confirmation on demo checkout so I know whether my order succeeded.              | **F3:** Simulated checkout form requiring a selected size and valid demo email format (`demo@example.test`), returning an inline error on missing/invalid input or an order ID on success. | Submit with no size or invalid email $\rightarrow$ error alert displays and nothing saves. Submit with valid size + email $\rightarrow$ confirmation banner with generated order number appears. |
| **S4** | As the store owner, I want demo orders saved in a real SQLite database so order history persists across server restarts. | **F4:** Local Node server (`server.mjs` using built-in `node:sqlite`) that validates inputs, calculates totals server-side (`qty × 38`), and persists orders in SQLite (`data/orders.db`). | Place a demo order, stop `node server.mjs` (`Ctrl + C`), restart the server, refresh the page, and confirm the previous order ID still renders in "Recent Demo Orders."                          |

### Data, States & SQLite Implementation Plan

- **Inputs & Limits:** Size (`S`, `M`, `L`, `XL`), quantity (`1–5`), and demo email (`demo@example.test`, validated only, never stored permanently). Fictional brand; unverified fabric GSM/shrinkage figures remain excluded per product boundary.
- **UI States:** `idle` $\rightarrow$ `validation-error` (missing size/bad email) $\rightarrow$ `submitting` $\rightarrow$ `confirmed` (with SQLite order ID) $\rightarrow$ `server-error` (if backend write fails).
- **SQLite Backend Plan:** Extend `server.mjs` using Node's native `node:sqlite` (`DatabaseSync`) following the course _Campus Cotton_ SQLite starter pattern (`POST /api/orders` to insert validated orders and `GET /api/orders` to list saved orders). Server calculates price from its own constant (`38`) rather than trusting client-submitted totals. Note: Static GitHub Pages preview cannot execute SQLite and will display a clear notice that persistence requires running `npm start` locally.
- **AI Help:** Gemini assisted in structuring the comparison table and SQLite endpoint plan; all brand decisions, user stories, and checks were verified against `docs/research.md` and `SPEC.md`.
- **SQLite Backend Plan:** Extend `server.mjs` using Node's native `node:sqlite` (`DatabaseSync`) following the course _Campus Cotton_ SQLite starter pattern (`POST /api/orders` to insert validated orders and `GET /api/orders` to list saved orders). Server calculates price from its own constant (`38`) rather than trusting client-submitted totals. Added `data/` and `*.db` to `.gitignore` so local test order databases are never committed to GitHub. Note: Static GitHub Pages preview cannot execute SQLite and will display a clear notice that persistence requires running `npm start` locally.

## Evidence

- Storefront branding, two visual direction previews, and verified baseline specs updated in `public/index.html` and `public/styles.css`.
- Automated test meaning, keyboard/mobile browser observations, and keep/change decisions recorded in [LEARNING.md](LEARNING.md#storefront-revision--verification-log-same-shirt-different-story).

| Spec ID   | Files                                                                   | Issue / PR       | Actual checks and observations                                                                                                                                       |
| :-------- | :---------------------------------------------------------------------- | :--------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BRAND-001 | `public/index.html`, `public/styleguide.html`, `SPEC.md`, `LEARNING.md` | Issue #1 / PR #1 | Prepared checks: `npm run check` passed. Browser verification: size selector and bag operational, responsive mobile layout verified, full keyboard tab order intact. |
