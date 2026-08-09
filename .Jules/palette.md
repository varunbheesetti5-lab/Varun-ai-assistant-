# Palette's UX Journal

## 2023-11-20 - Robust Text-Copying in Nested Code Elements
**Learning:** In dynamically styled message bubbles where elements like "Copy" buttons are appended inside container tags (e.g., `<pre>`), querying `pre.textContent` or `pre.innerText` directly can inadvertently copy the copy button's text (e.g. "📋 Copy") along with the actual code. Separating code into a dedicated nested tag (like `<code>`) and targeting it using `pre.querySelector('code').innerText` avoids copying UI elements and preserves correct line breaks.
**Action:** Always target the specific innermost node holding the text (e.g., `code`) inside a larger block (e.g., `pre`) when implementing clipboard logic, ensuring no dynamically added control elements are copied.
