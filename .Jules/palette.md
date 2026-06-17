## 2025-05-15 - Chat Accessibility and Dynamic Feedback
**Learning:** For chat interfaces, using `aria-live="polite"` and `role="log"` on the message container is essential for notifying screen reader users of new content. Additionally, dynamic interactive elements like "Copy" buttons should provide both visual (tooltips/titles) and programmatic (ARIA labels) feedback when their state changes (e.g., from "Copy" to "Copied!").
**Action:** Always include live regions for message-based UIs and ensure dynamic buttons update their `aria-label` and `title` to reflect state changes.
