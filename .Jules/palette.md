## 2026-07-20 - Preventing HTML Hardcoded Disabled State False-Positives
**Learning:** Hardcoding a 'disabled' attribute directly in HTML can lead to misunderstanding during review processes (or fallback bugs if script initialization fails) if the element is dynamically managed. It is safer and clearer to perform initial disabling programmatically within the initialization script.
**Action:** Configure default interactive states dynamically inside initialization JavaScript instead of hardcoding 'disabled' directly in static HTML.

## 2026-07-20 - Precise Inner Code Copying in Chat Pre-formatted Blocks
**Learning:** Copying a `<pre>` block that contains dynamically appended elements (like a Copy button) using `pre.textContent` captures all inner child text, including the copy button label itself. Targeting the inner `<code>` element with `.innerText` correctly isolates only the formatted code content.
**Action:** Use `const codeElement = pre.querySelector('code'); const textToCopy = codeElement ? codeElement.innerText : pre.textContent;` to robustly preserve code formatting and newlines without capturing sibling UI controls.
