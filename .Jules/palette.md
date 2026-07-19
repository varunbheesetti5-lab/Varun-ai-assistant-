# Palette's Journal

🎨 A log of critical UX/accessibility insights and learnings for Varun AI Assistant.

## 2024-07-19 - [Robust Code Block Copying in Custom Markdown Renderers]
**Learning:** In custom client-side Markdown renderers where newlines are replaced with `<br>` tags globally, standard `element.textContent` fails because it ignores `<br>` elements when retrieving the text nodes, leading to copied code blocks losing all line breaks. Additionally, querying `pre.textContent` captures any dynamically appended child element text (such as the text on a Copy button). Using `element.innerText` inside the inner `<code>` element solves both problems by correctly interpreting `<br>` as `\n` while isolating the code text from any sibling copy controls.
**Action:** Always target the specific nested code-holding element (e.g., `code` tag inside a `pre` container) and utilize `innerText` rather than `textContent` when the renderer replaces literal `\n` characters with markup elements, ensuring perfect formatting extraction and ignoring sibling interactive controls.
