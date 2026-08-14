## 2024-08-14 - Isolated Dynamic Code Copying

**Learning:** When dynamic utility overlays (like a copy-to-clipboard button) are appended directly inside a `<pre>` container, using the parent's `.textContent` will capture the overlay's text (e.g. "📋 Copy" or "✅ Copied!") into the clipboard. This results in bad UX where button content is included in code copy/paste operations. Utilizing `.innerText` on the specific child `<code>` element cleanly isolates only the raw code block and preserves line breaks correctly without capturing sibling interactive components.

**Action:** When designing code-copying utility buttons within `<pre>` elements, target the specific raw content element (e.g., `code`) using `.innerText` instead of retrieving the `.textContent` of the main container, preventing button text leakage.
