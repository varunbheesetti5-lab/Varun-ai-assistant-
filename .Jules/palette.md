## 2024-05-27 - [Accessibility for Single-File Chat Apps]
**Learning:** In minimalist chat interfaces, dynamic content such as message history and typing indicators must explicitly use `aria-live="polite"` and `role="status"` to ensure screen reader users are notified of updates without interruption.
**Action:** Always include ARIA live regions and appropriate roles when adding dynamic feedback elements like typing indicators or message streams.
