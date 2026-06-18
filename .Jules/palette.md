## 2024-06-18 - Standardizing Accessibility Utilities in Single-File Projects
**Learning:** In minimal single-file projects without CSS frameworks (like Tailwind or Bootstrap), essential accessibility utilities like `.sr-only` are often missing, leading to reliance on placeholders instead of proper labels.
**Action:** Always verify the existence of a screen-reader-only utility before adding accessible labels, and implement a standard `.sr-only` class if missing to support visually hidden but ARIA-compliant elements.
