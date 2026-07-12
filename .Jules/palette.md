## 2026-07-12 - [Code Block Copy Accessibility]
**Learning:** In single-file applications where copy buttons are appended to `<pre>` tags, `pre.textContent` includes the text of the button itself. Using `pre.querySelector('code').textContent` ensures only the code is copied, and updating ARIA labels programmatically provides necessary feedback to assistive technology.
**Action:** Always target the inner `<code>` element for clipboard operations and sync ARIA labels with visual state changes.
