## 2026-06-16 - Robust Copy-to-Clipboard for Code Blocks
**Learning:** Standard `pre.textContent` can inadvertently include the text of UI elements like "Copy" buttons if they are nested within the `pre` tag. This results in "Copy" being prepended or appended to the actual code in the user's clipboard.
**Action:** Clone the target element, programmatically remove interactive sub-elements (like buttons), and then extract `textContent` from the cleaned clone to ensure only the intended code is copied.
