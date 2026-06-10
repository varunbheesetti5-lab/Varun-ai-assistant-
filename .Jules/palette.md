## 2025-05-14 - [Chat Accessibility and Feedback]
**Learning:** In a chat interface, screen readers need explicit roles (`role="log"`) and live regions (`aria-live="polite"`) to announce new messages automatically. Additionally, interactive feedback for actions like "Copy" must be both visual and audible (via `aria-label` updates).
**Action:** Always include ARIA live regions for message logs and provide dual visual/audible feedback for common utility actions.
