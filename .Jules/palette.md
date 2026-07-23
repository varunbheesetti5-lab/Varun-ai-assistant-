# Palette UX Journal

## 2024-11-23 - Dynamic Code Block Focus Management
**Learning:** Dynamically injected elements, such as 'Copy' buttons in generated markdown code blocks, are frequently missed in accessibility reviews. While standard elements have static stylesheets, dynamic buttons require custom inline focus indicators or globally-scoped selector definitions to ensure keyboard users maintain logical tab order and a clear focus-visible state.
**Action:** When injecting interactive elements dynamically into the DOM, always define matching global CSS focus rules or inject explicit outline style handlers, and use matching `aria-label` and `title` attributes for full screen-reader and mouse-user clarity.
