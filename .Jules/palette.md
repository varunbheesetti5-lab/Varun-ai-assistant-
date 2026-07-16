## 2025-05-15 - Precise Code Copy Logic
**Learning:** In code blocks where UI elements (like copy buttons) are appended to the `<pre>` tag, using `pre.textContent` incorrectly includes the button's text in the clipboard.
**Action:** Use `pre.querySelector('code').textContent` or clone the element and remove non-code children before extracting text to ensure only the code is copied.
