## 2026-07-01 - [Surgical Clipboard Target Selection]
**Learning:** When adding interactive UI elements (like a "Copy" button) into a container whose text content is the target of an action, using `textContent` on the container will include the text of the UI elements themselves.
**Action:** Always use a specific selector (like `pre code`) or clone the element and remove UI elements before extracting text to ensure the clipboard content is clean.
