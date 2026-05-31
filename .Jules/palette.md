## 2026-05-31 - [Accessibility enhancements for Chat]
**Learning:** Icon-only buttons and dynamic regions (like typing indicators and message logs) need explicit ARIA labels and live region attributes to be accessible to screen reader users.
**Action:** Always include 'aria-label', 'role="status"', and 'aria-live="polite"' when building interactive chat interfaces.
