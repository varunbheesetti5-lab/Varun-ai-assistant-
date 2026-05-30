## 2026-05-30 - Accessibility and Micro-UX Enhancements

**Learning:** In projects where custom CSS is discouraged, `aria-label` is a valid and preferred alternative to visually hidden `<label>` elements with utility classes like `.sr-only`. Also, when implementing "copy to clipboard" buttons within code blocks, it's crucial to target the specific `code` element to avoid copying the button's own text.

**Action:** Prefer `aria-label` for simple labeling needs to stay within CSS boundaries. Always verify the scope of text being copied in "copy to clipboard" features.
