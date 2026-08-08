# Palette's Journal

## 2024-08-08 - Initial UX Review and Planning
**Learning:** Icon-only buttons (like `#sendButton` and dynamically added "Copy" buttons) lack clear visual text, making them inaccessible to screen readers and difficult to discover for some users unless they have explicit `aria-label` and `title` tooltip attributes. Additionally, dynamic content changes (like "Thinking" status or dynamic copying feedback) require polite ARIA alerts (`aria-live="polite"`) to be properly broadcasted. Finally, copying from code blocks using `pre.textContent` accidentally grabs the copy button's own text if the button is appended inside the `pre` element.
**Action:** Implement robust target selection (`pre.querySelector('code')`) for code block copying, add `.sr-only` CSS class and corresponding `<label>` for `#messageInput`, and supply appropriate `aria-label` and `title` attributes on all icon-only interactions.
