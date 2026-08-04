# Palette's UX & Accessibility Journal

## 2026-03-24 - Unlinked Form Labels & Non-Descriptive Modal Controls
**Learning:** Found a widespread accessibility issue across both the main landing page (`index.html`) and the dedicated checkout flow (`checkout.html`). While forms had visual text tags using `<label>` and inputs had appropriate placeholders, they were not structurally linked via `for`/`id` attributes. Additionally, modal close buttons and cart control buttons relied entirely on text content like "×", "−", and "+", causing screen readers to mispronounce or ignore critical layout controls.
**Action:** Link all `<label>` elements to their corresponding input/select/textarea controls using the `for` attribute and ensure all interactive icons and close buttons have descriptive `aria-label` tags.
