# Bolt's Performance Journal

## 2024-11-20 - [Scroll Event DOM Overhead]
**Learning:** In a single-page HTML architecture, continuous and un-throttled scroll event handlers that repeatedly query the DOM and write state to class lists cause severe scroll jank and continuous style/layout recalculations.
**Action:** Cache the required DOM element and use a state flag to ensure DOM manipulation and styling class toggles only occur when the scroll threshold state actually transitions.
