## 2026-06-04 - [Selective Clipboard Copying]
**Learning:** When adding interactive elements like "Copy" buttons to code blocks, using `textContent` on the parent container (e.g., `pre`) will include the button's own text in the clipboard.
**Action:** Target the specific content element (e.g., `code`) or exclude UI elements when reading text for clipboard operations.
