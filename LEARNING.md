# Learning record

This file is a brief record of decisions, evidence, and assistance received for IS117 Brand Studio.

## Checkpoint summary

- **Audience & Need:** Identified primary persona as remote software engineers needing zero decision fatigue and clean collar durability on camera. Contrasting secondary persona is students needing wash longevity.
- **Brand Identity:** Established NULLSET under The Sage archetype with unadorned, deliberate, and objective voice traits.
- **Visual Direction:** Modernist grid layout chosen for high clarity, readability, and immediate spec inspection.
- **Ethical Persuasion:** Implemented spec transparency and wash stability metrics without false scarcity or fabricated reviews.
- **Automated & Manual Checks:** Automated lint and test suites executed via `npm run check`. Manual browser verification performed for size selection, bag state, mobile viewport wrapping, and keyboard focus order.

## Current research checkpoint

- **AI assistance (learner-reviewed for summary accuracy):** On November 8, 2026, the AI checked official page content from Lady White Co., Outlier, and Asket and drafted source-linked observations and positioning hypotheses in [docs/research.md](docs/research.md). The learner confirmed this summary is accurate; that confirmation does not make the AI observations customer findings or learner research. The learner's own site observations, peer feedback, and response to that feedback are not yet recorded in this chat.

## Storefront Revision & Verification Log (Same Shirt, Different Story)

### 1. Meaning of One Automated Test

- **Test Inspected:** `page integrity and automated accessibility: /` (`tests/browser/studio.spec.js:61`)
- **What It Actually Checks:** Launches Chromium via Playwright against the live local server, verifies zero HTTP 404 asset failures (such as missing stylesheets or scripts), and runs `axe-core` against WCAG 2.0 A/AA and WCAG 2.1 AA rules. Specifically, it mathematically verifies that every text node meets at least a 4.5:1 foreground-to-background contrast ratio and that landmarks (`<header>`, `<main>`, `<footer>`, `<nav>`) and form labels are programmatically valid.
- **Why It Matters:** Passing this test confirms that neither the primary slate theme (`#2B3A42` on `#FAF9F6`) nor the warm editorial preview (`#2C2520` on `#F3EFEA`) introduces unreadable text or broken asset paths.

### 2. Real Browser Observations (Keyboard & Mobile)

- **Keyboard Navigation (Desktop Chromium):** Pressing `Tab` from the browser address bar immediately reveals the `Skip to main content` link with a high-contrast `#005FCC` focus ring. Continuing with `Tab` moves cleanly through the NULLSET logo, navigation links, radio size options (`S`, `M`, `L`, `XL` selectable via arrow keys), `Add to Demo Bag` button, and `Empty Bag` control without keyboard traps.
- **Mobile Viewport (375px Width):** At 375px narrow width, `.product-page` and `.directions-grid` collapse cleanly into single-column stacks (`grid-template-columns: 1fr`). Size pills wrap cleanly without horizontal page overflow, and both visual direction cards remain legible without clipping.

### 3. Decisions: What Was Kept vs. Changed

- **Kept:**
  - The restrained Sage palette (`#FAF9F6` background, `#111` ink, `#2B3A42` slate accent) and single-SKU white T-shirt scope.
  - The accessible form validation and session-only demo bag behavior in `shop.js`.
- **Changed:**
  - Replaced the neutral starter storefront copy and header in `public/index.html` with the NULLSET geometric SVG mark, issue eyebrow (`ISSUE 01 // STANDARD UNIFORM`), and brand positioning copy.
  - Added a side-by-side **Visual Direction Comparison** section on `index.html` contrasting Direction A (Deliberate Everyday Uniform) against Direction B (Lifestyle-Led Minimalist).
  - Removed unverified fabric GSM and post-wash shrinkage claims from `index.html` and `docs/research.md`, explicitly labeling material/wash metrics as pending supplier verification to adhere to `SPEC.md` product boundaries.
