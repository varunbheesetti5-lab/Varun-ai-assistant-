
## 2024-05-23 - [Accessibility: ARIA Live Regions for Chat]
**Learning:** In a single-page AI chat application, dynamic content updates (like 'AI is thinking' or new messages) are not automatically announced by screen readers.
**Action:** Use 'aria-live="polite"' on message containers and status indicators to ensure screen reader users receive timely updates without interrupting their current flow. Add 'role="log"' to the message history to provide semantic context for assistive technologies.
