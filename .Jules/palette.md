# Palette's Journal - Critical Learnings Only

This journal contains critical UX and accessibility insights discovered during design and development.

## 2024-08-04 - Code Block Clipboard Extraction Isolation
**Learning:** Querying the `textContent` of a parent `<pre>` element for copy operations can accidentally capture child interactive UI elements (such as the copy button itself, i.e., copying "📋 Copy" or "✅ Copied!"), especially when the copy button is dynamically appended inside the `<pre>` container. Furthermore, `textContent` does not preserve line-break formatting from `<br>` tags accurately compared to `innerText`.
**Action:** When implementing code copy functionality, isolate the copy target by querying the inner `<code>` element directly (`pre.querySelector('code')`) and use its `.innerText` property to guarantee that only the code itself is copied, preserving format and excluding sibling UI controls.
