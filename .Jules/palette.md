# Palette's UX & Accessibility Journal

## 2026-08-08 - Escape Key Integration & ARIA Labels for Overlays
**Learning:** In highly customized SPA architectures without a UI framework, separate overlay elements (like drawers, modal popups, and sidebars) often implement independent open/close logic. It is common to miss adding unified keyboard handlers (e.g., `Escape` key dismissals) and ARIA accessibility labels (`aria-label`) on close buttons that use non-semantic character symbols (like `×`).
**Action:** Always audit monolithic or multi-component single page applications for overlay/modal instances and ensure they all wire into a unified keyboard navigation handler. Always ensure all "close" button variants using standard symbols contain clear descriptive ARIA labels to be screen-reader compliant.
