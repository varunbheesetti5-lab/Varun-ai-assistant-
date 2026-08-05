# Palette's Journal

## 2024-03-15 - Initial Journal Setup
**Learning:** Accessibility and delightful micro-interactions are core pillars of a great user interface. Small touch-ups, such as proper ARIA attributes, keyboard accessibility, focus indicators, and visual feedback states, make an application feel professional and easy to navigate for all users.
**Action:** Always verify keyboard focus styles, use existing UI tokens/colors, write semantic markup, and format PR titles as '🎨 Palette: [UX improvement]'.

## 2026-08-05 - Consistent Interactive Tooltips & ARIA Updates for Dynamic Actions
**Learning:** For icon-only buttons (such as 'Send Message' and code block 'Copy' buttons), supplying both an `aria-label` and matching `title` attributes provides a consistent UX for both keyboard screen-readers and visual mouse-over users. Furthermore, when the button state dynamically updates (e.g., from 'Copy' to 'Copied!'), both of these attributes should be updated simultaneously to reflect the state change uniformly.
**Action:** Always bundle `aria-label` and `title` updates together when implementing dynamic, interactive button feedback states.
