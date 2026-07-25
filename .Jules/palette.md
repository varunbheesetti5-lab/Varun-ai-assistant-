# Palette's UX Journal

This journal logs critical UX and accessibility learnings and design choices.

## 2025-07-25 - [Accessible Dynamic Copy Button and Status Indicators]
**Learning:** In a single-file application structure where UI elements (such as copy-code buttons inside <pre> blocks) are dynamically constructed via JavaScript inside string templates or DOM APIs, we must be extra vigilant about:
1. Dynamic copy button implementations fetching `pre.textContent`, which accidentally includes the button's own text (e.g., "📋 Copy") in the copied text. By targeting `pre.querySelector('code')` and using its `innerText`, we ensure only the actual code block is copied.
2. Accessibility of icon-only elements: Buttons like "▶" and "Copy" need explicit `aria-label` and `title` attributes (providing tooltips on hover for mouse users and semantic labels for screen readers).
3. Status announcements: Dynamic/async elements (such as `#apiStatus` and `#typingIndicator`) must use `aria-live="polite"` to proactively notify screen-reader users of state changes without interrupting their workflow.
**Action:** Always inspect custom rendered code blocks and icon buttons for accessible labeling, tooltips, and correct DOM/text extraction logic, and guarantee that dynamic status components use proper live regions.
