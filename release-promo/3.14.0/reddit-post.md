**Title:** Cline v3.14 Released: Improved Gemini Caching, `/newrule` Command, Enhanced Checkpoints & More!

Hey everyone,

Excited to share Cline v3.14 is out! This release focuses on refining the core experience based on community feedback, tackling some key pain points, and adding useful new features.

Here are the highlights:

**Improved Gemini Caching & Transparency**

We know cost tracking and efficiency with Gemini models have been tricky. v3.14 brings:

*   **More Robust Caching:** Refined logic for Gemini and Vertex providers for better reliability and cost savings.
*   **Cache UI (OpenRouter/Cline):** Added visibility into when caching is active for these providers. `[VISUAL: Cache UI Screenshot]`
*   **Pricing Calculation Enabled:** Better cost estimates for Gemini/Vertex during usage.

**More Flexibility with Enhanced Checkpoints**

We've added more checkpoints across the task workflow:

*   **Plan-to-Act Checkpoint:** Most importantly, a checkpoint is now created right when you switch from Plan to Act mode. Easily revert to the planning stage if the initial code generation isn't right, without losing history. `[VIDEO: Checkpoint Demo]`
    *   *Pro Tip:* Don't hesitate to use this! Refining the plan early is often faster than editing lots of generated code.

**Generate Project Standards with `/newrule`**

Need to document project standards like design systems or coding conventions?

*   Use the `/newrule` slash command (e.g., `/newrule create design system guidelines`). Cline analyzes your project context and generates a `.clinerules` file documenting the standards, ensuring consistency. `[VIDEO: /newrule Demo]`
    *   *Pro Tip:* Ask Cline to document API patterns, testing conventions, tech stack summaries, and more!

**LaTeX Rendering (v3.14 Special)**

*   Fitting for v3.14, Cline now fully renders LaTeX markup in the chat! `[VISUAL: LaTeX Rendering Example]`

**Key Quality-of-Life Updates & Community Contributions**

*   **Improved Drag & Drop:** Drag files from your OS file explorer directly into Cline (Remember to **hold Shift**!). `[VISUAL: Drag & Drop Example]`
*   **Copy Buttons:** Added to code and markdown blocks (Thanks **@weshoke**!). `[VISUAL: Copy Button Example]`
*   **Batch History Deletion:** Select and delete multiple tasks at once (Thanks **@danix800**!). `[VISUAL: Batch History Deletion Demo]`
*   **Custom Timeouts:** Configure API request timeouts for OpenRouter/Cline & Ollama (Thanks **@WingsDrafterwork**!).
*   **Bedrock Updates:** Support for custom model IDs (Thanks **@clicube**!) & Amazon Titan Text Premier (Thanks **@watany**!).
*   **Fixes:** Addressed terminal race conditions, Windows path handling (Thanks **@DaveFres**!), local dev syntax errors (Thanks **@DaveFres**!), git commit mentions, cost calculations (Thanks **@BarreiroT**!), and more.

Huge thanks to all community contributors! 🙏

**Get Started**

Update Cline via the VS Code Marketplace.

Read the full details in our [latest blog](https://cline.bot/blog/cline-v3-14-improved-gemini-caching-newrule-command-enhanced-checkpoints-key-updates)
See the announcement thread on [X](https://x.com/cline/status/1918694300164239753)
Check out the full [changelog](https://github.com/cline/cline/blob/main/CHANGELOG.md) for all the details.

Let us know what you think here or on [Discord](https://discord.gg/cline)!
