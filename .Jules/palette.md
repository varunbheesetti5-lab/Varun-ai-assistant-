## 2026-05-29 - [Accessibility and Interaction Feedback for Chat Interfaces]
**Learning:** Chat interfaces benefit greatly from 'aria-live="polite"' on typing indicators and 'role="status"' on connection indicators. Visual feedback for async actions (like changing a button icon to '⌛') provides immediate reassurance to users, especially when the main app container is dimmed.
**Action:** Always include ARIA live regions for dynamic status updates and ensure icon-only buttons have descriptive 'aria-label' attributes. Use 'try...finally' to ensure UI state consistency.

## 2026-05-29 - [Environment Specific: Serving extensionless files]
**Learning:** The 'html' file in this repo is extensionless and uses CRLF line endings. Python's 'http.server' serves it as 'application/octet-stream', which causes Playwright to download it rather than navigate.
**Action:** Copy the file to 'index.html' for verification purposes to ensure it is served as 'text/html'. Be mindful of CRLF when using string replacement tools.
