Cline v3.14 is live.

Here's what's new 🧵 ↓
*(Image accompanying this tweet should list: Improved Gemini Caching, Plan-to-Act Checkpoints, /newrule Slash Command, LaTeX Rendering)*

---

First up, we've made significant improvements to Gemini caching & transparency.
- Refined caching logic for Gemini/Vertex providers for better reliability & cost savings.
- Added a Cache UI for OpenRouter/Cline providers for visibility. `[VISUAL: Cache UI Screenshot]`
- Enabled pricing calculations for Gemini/Vertex.

---

Checkpoints are now more flexible. We added more checkpoints across the task, including right when switching from Plan to Act mode.

This lets you easily revert to the planning stage if the initial code generation isn't quite right, offering more granular control. `[VIDEO: Checkpoint Demo]`

> Pro Tip: Refining the plan early is often faster than editing lots of generated code!

---

Need project standards documented? Ask Cline to generate them with the new /newrule command!

e.g., "/newrule create design system guidelines". Cline analyzes project context (code, libs, patterns) & generates a .clinerules file to ensure consistency. `[VIDEO: /newrule Demo]`

> Pro Tip: Use it for API patterns, testing conventions, tech stack summaries & more!

---

Fitting for v3.14, we've added full LaTeX rendering support!

Cline now correctly renders math equations and other LaTeX markup directly in the chat. `[VISUAL: LaTeX Rendering Example]`

---

This release also includes key QoL updates:
- Copy Buttons: Added to code & markdown blocks (Thanks @weshoke!). `[VISUAL: Copy Button Example]`
- Improved Drag & Drop: Drag files directly from your OS file explorer (Remember to hold Shift!). `[VISUAL: Drag & Drop Example]`
- Batch History Deletion: Select & delete multiple tasks (Thanks @danix800!). `[VISUAL: Batch History Deletion Demo]`

---

Other updates include:
- Custom Timeouts: Configurable API request timeouts for OpenRouter/Cline & Ollama (Thanks @WingsDrafterwork!).
- Bedrock Updates: Support for custom model IDs (Thanks @clicube!) & Amazon Titan Text Premier (Thanks @watany!).
- Fixes: Addressed terminal race conditions, Windows paths (@DaveFres!), local dev syntax (@DaveFres!), git mentions, cost calculations (@BarreiroT!), & more.

Huge thanks to all community contributors! 🙏

---

Update Cline via the VS Code Marketplace to get v3.14.

Read the full details on the blog: https://cline.bot/blog/cline-v3-14-improved-gemini-caching-newrule-command-enhanced-checkpoints-key-updates
Changelog: https://github.com/cline/cline/blob/main/CHANGELOG.md

Let us know what you think!
