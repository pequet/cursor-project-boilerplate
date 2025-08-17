---
description:  
applyTo: "**/*.instructions.md,*.instructions.md"
---

# 260: `.github/instructions` Frontmatter Editing Limitation

### AI Limitation Reminder
You cannot reliably add or modify the YAML frontmatter of existing `.github/instructions` files. Attempts often fail silently.

### Required Protocol
WHEN a task involves modifying the frontmatter of an existing `.github/instructions` file (e.g., adding `globs`, changing `description`):

1.  **ACKNOWLEDGE LIMITATION:** State that you cannot reliably perform the frontmatter edit.
2.  **RECOMMEND MANUAL EDIT:** Advise the user to perform the edit manually.
3.  **OFFER CONTENT ASSISTANCE:** Offer to draft or modify the Markdown *content* (the text below the `---` frontmatter closing).
4.  **HANDLE NEW FILES CORRECTLY:** When creating *new* `.github/instructions` files, always include the complete and correct frontmatter from the start.

### Rationale for Protocol
This protocol is based on observed tool behavior where `edit_file` does not consistently apply changes to `.github/instructions` file frontmatter. Following these steps prevents repeated failed attempts and sets correct user expectations.
