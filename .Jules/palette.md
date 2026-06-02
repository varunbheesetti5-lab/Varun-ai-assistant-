## 2026-06-02 - [Accessibility in Dynamic Chat Interfaces]
**Learning:** For chat interfaces, visual changes like new messages or typing indicators are not automatically announced to screen readers.
**Action:** Use `aria-live="polite"` on message containers and `role="status"` on typing indicators to ensure inclusive communication. Also, ensure dynamically created elements like "Copy" buttons have programmatic accessibility labels.
