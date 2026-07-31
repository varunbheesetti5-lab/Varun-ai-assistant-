# Palette's UX Journal

## 2025-07-31 - Robust Code Copying and Screen Reader Support
**Learning:** Copying text from a container block (such as `<pre>`) using `pre.textContent` can inadvertently capture the text of dynamically appended child elements, such as absolute-positioned Copy buttons (e.g., capturing 'Copy' or 'Copied!' inside the code text). For correct behavior, always extract text from the specific child text element (e.g., `<code>`) using `innerText` to preserve formatting, line breaks, and prevent copying button labels.
**Action:** Always scope clipboard extractions precisely to the inner `<code>` element, and dynamically update both `aria-label` and `title` attributes on interactive elements to provide consistent audio and visual hover states.
