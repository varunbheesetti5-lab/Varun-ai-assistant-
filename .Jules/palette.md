## 2026-06-12 - Robust Clipboard Copy in Chat Interfaces
**Learning:** In chat interfaces where UI elements (like "Copy" buttons) are injected into code blocks, using `textContent` directly on the parent element for clipboard actions can accidentally include the button text (e.g., "console.log('hello')Copy").
**Action:** When implementing copy-to-clipboard, always clone the target element and programmatically remove any UI-only child elements (buttons, tooltips) before extracting the text content for the clipboard.
