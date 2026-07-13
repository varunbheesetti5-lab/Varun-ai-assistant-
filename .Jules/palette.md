## 2025-05-14 - Robust Clipboard Extraction in Single-File AI Apps
**Learning:** In applications where code blocks are dynamically generated with "Copy" buttons appended to the `<pre>` tag, using `pre.textContent` for clipboard operations inadvertently includes the "Copy" text itself.
**Action:** Always target the specific `<code>` element within the `<pre>` tag for text extraction (`pre.querySelector('code').textContent`) to ensure only the code is copied, and provide immediate ARIA label updates for screen reader feedback.
