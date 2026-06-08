## 2026-06-08 - [Improving Async Feedback and Screen Reader Support]
**Learning:** For chat interfaces, combining `aria-live="polite"` on the message container with visual loading indicators (like a button icon change) creates a more inclusive experience by providing both auditory and visual feedback during async operations.
**Action:** Always pair visual state changes (like '⌛' icons) with appropriate ARIA live regions and ensure these states are properly reset using `finally` blocks to prevent the UI from becoming unresponsive to assistive technology.
