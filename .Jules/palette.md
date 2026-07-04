# Palette's Journal - Critical UX/Accessibility Learnings

## 2025-07-04 - Accessibility and Copy-to-Clipboard Patterns
**Learning:** When adding interactive elements like "Copy" buttons inside container elements (e.g., `<pre>`), using `container.textContent` for the clipboard will inadvertently include the text of the button itself. This creates a poor user experience by polluting the copied content.
**Action:** Always target the specific content element (e.g., `pre.querySelector('code')`) or clone the element and remove UI components before extracting text for the clipboard.
