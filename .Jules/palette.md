# Palette UX Journal

## 2026-08-06 - Preventing UI Text Pollution in Code Block Clipboard Copying
**Learning:** Appending copy button elements directly to container parent elements (e.g., `<pre>`) pollutes the container's `textContent` with the button's own text (e.g., "Copy"). Utilizing `querySelector('code')` to target the code element and accessing its `innerText` ensures clean code copying without capturing auxiliary interactive buttons.
**Action:** Always target the innermost code block node (like `code`) rather than the container parent when copying text, and set explicit `aria-label` and matching `title` attributes on both initial render and dynamic click states for comprehensive tooltip and screen reader updates.
