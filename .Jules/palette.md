## 2026-06-05 - [Accessibility & Feedback Enhancements]
**Learning:** Screen readers require explicit labels for inputs even when placeholders are present. Using an `.sr-only` class allows for accessible labeling without affecting the visual design. Visual feedback for async actions (like changing a button icon to a loading state) significantly improves the perceived responsiveness of the app.
**Action:** Always include `.sr-only` labels for form inputs and provide clear visual/ARIA feedback for all asynchronous state changes.

**Learning:** When adding interactive elements (like 'Copy' buttons) dynamically to the DOM, they must include appropriate `aria-label` attributes to be accessible to screen reader users.
**Action:** Programmatically set `aria-label` when creating elements via JavaScript.

**Learning:** Targeted copy-to-clipboard functionality must be careful not to include UI text (like the text of the 'Copy' button itself). Targeting the specific content element or cloning and stripping UI elements ensures a clean clipboard.
**Action:** Use `pre.querySelector('code').textContent` or clone/strip UI elements before copying to clipboard.
