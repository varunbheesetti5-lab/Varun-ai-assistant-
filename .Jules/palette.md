## 2025-05-14 - [Accessibility & Feedback in Single-File Apps]
**Learning:** Single-file HTML applications often lack basic accessibility (ARIA labels, live regions) and visual feedback for async operations. Utility classes like `.sr-only` are essential for providing context to screen readers without breaking the visual design.
**Action:** Always include a `.sr-only` utility and use `try...finally` blocks to manage UI state changes (e.g., loading icons) during async requests to ensure the interface remains consistent even on failure.
