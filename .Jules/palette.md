## 2026-07-10 - Accessibility for Icon-only Buttons and Inputs
**Learning:** Icon-only buttons and textareas with only placeholders lack sufficient context for screen readers. Using ARIA labels and visually hidden labels (.sr-only) ensures accessibility without compromising the minimalist aesthetic.
**Action:** Always provide explicit <label> (can be .sr-only) for form inputs and aria-label for icon buttons.

## 2026-07-10 - Robust Clipboard Interaction Feedback
**Learning:** Users need immediate feedback after copying content. Updating the button text and ARIA label to "Copied!" provides both visual and assistive technology confirmation.
**Action:** Implement dynamic ARIA label updates alongside visual text changes for all interactive feedback loops.
