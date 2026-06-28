## 2026-06-28 - [Accessible Code Copy Pattern]
**Learning:** When adding interactive elements like "Copy" buttons inside `<pre>` tags, using `pre.textContent` can inadvertently include the button's own text in the clipboard. Using `pre.querySelector('code').textContent` (if available) ensures only the intended code is copied while allowing the button to remain a sibling or child of the code container for positioning.
**Action:** Always target the specific code element (e.g., `<code>`) within a container when implementing copy-to-clipboard functionality to avoid capturing UI labels.
