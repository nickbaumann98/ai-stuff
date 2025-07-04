Just pushed Cline v3.13.2 -- this patch release Gemini provider performance with caching, adds thinking budget support, and includes the Gemini 2.5 Flash model.

Here's the breakdown: 🧵

---

Also in this release:
- Support for `!include .file` directive in `.clineignore`
- Improved slash command functionality
- Better prompting for the new task tool (better summaries of your context!)

---

Key fixes include:
- Correct o1 temperature for Azure API
- Functional "add new rule file" button
- Increased Ollama provider timeout
- Better non-UTF-8 file handling

---

More fixes:
- Settings no longer reset when changing providers
- Commas added to terminal outputs
- Terminal errors from non-alphanumeric outputs resolved
- Auto-approve settings persistence fixed
- Mermaid syntax error in docs fixed

---

And finally, browser use is now supported through any model that handles images, removing the `supportsComputerUse` restriction.

Update Cline in VS Code to get the latest improvements!
