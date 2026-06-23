## 2025-05-14 - Chat Interface Accessibility
**Learning:** Chat interfaces require `aria-live="polite"` and `role="log"` on the message container to ensure new incoming messages are announced to screen reader users. Additionally, dynamic UI feedback (like "Copied!") must be reflected in `aria-label` and `title` attributes to be accessible.
**Action:** Always implement `role="log"` and `aria-live` for sequential content logs, and programmatically update ARIA labels when element states change.
