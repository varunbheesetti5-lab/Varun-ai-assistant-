## 2026-06-24 - Accessibility and Feedback in Chat Interfaces

**Learning:** Chat interfaces often lack appropriate ARIA roles and live regions, making it difficult for screen reader users to track conversation flow. Additionally, icon-only buttons (like Send or Copy) provide no context without explicit ARIA labels, and placeholders are not a substitute for accessible labels. Providing visual feedback (like a loading icon) during async operations significantly improves the perceived responsiveness for all users.

**Action:** Always include `role="log"` and `aria-live="polite"` on message containers. Provide visually hidden `<label>` elements for inputs. Use `aria-label` and `title` for icon-only buttons, and implement loading states for long-running actions. Ensure "Copy" logic specifically targets content to avoid including UI text in the clipboard.
