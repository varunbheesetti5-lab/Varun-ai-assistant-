# Palette's UX Journal

## 2024-08-13 - [Isolate dynamic copy-paste elements from dynamic interactive buttons]
**Learning:** In dynamically styled chat applications, using simple element text retrieval APIs like `pre.textContent` for copying a code block introduces severe UX bugs by including nested UI elements such as dynamic copy button text ('📋 Copy' or '✅ Copied!'). Instead, isolating the code contents inside a nested semantic `<code>` tag using `code.innerText` guarantees only code is copied, and handles spacing formats cleanly.
**Action:** When designing code block layouts with embedded elements, always query for the target `code` tag specifically and read its `innerText` rather than grabbing container-level text content.
