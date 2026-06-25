## 2025-06-25 - Robust Accessibility for Standalone Chat Interfaces
**Learning:** For standalone single-file projects, micro-UX improvements like `aria-live` and `.sr-only` labels provide high impact with minimal code footprint. Combining `aria-label` with `title` ensures both screen reader accessibility and visual tooltips for icon-only buttons.
**Action:** Always include a `.sr-only` utility and apply it to labels for icon-heavy or minimalist inputs. Pair dynamic state changes (e.g., 'Copied!') with corresponding ARIA attribute updates for immediate assistive technology feedback.
