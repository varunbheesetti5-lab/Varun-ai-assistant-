## 2025-05-14 - Chat Interface Accessibility
**Learning:** For real-time chat interfaces, using `aria-live="polite"` and `role="status"` on status indicators (like API connectivity and typing indicators) ensures that state changes are announced to assistive technology users without disrupting the flow of the conversation. Additionally, icon-only buttons and textarea inputs must have accessible names via `aria-label` or hidden `<label>` elements.
**Action:** Always include `aria-live` on dynamic status elements and provide `.sr-only` labels for inputs that lack visible text labels.
