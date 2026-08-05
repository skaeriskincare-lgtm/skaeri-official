# Palette's UX & Accessibility Journal

## 2026-08-05 - Unified Keyboard Escape Listeners and Explicit Aria Labels for Monolithic SPAs
**Learning:** In highly monolithic single-page applications with multiple custom overlays (e.g., slide-out carts, checkout modals, product detail popups), global key event listeners for keyboard navigation must be exhaustive and unified. If keyboard shortcuts like `Escape` only close a subset of overlays, it breaks expectations and keyboard navigation. Additionally, custom close controls (such as multiplication symbols `×` or emojis) lack descriptive text and must be explicitly labeled with `aria-label` tags to ensure accessibility for screen readers.
**Action:** Always map the Escape key globally to cleanly close all active overlay screens and drawers, and ensure any custom/icon/emoji trigger buttons have clear `aria-label` tags for assistive technology.
