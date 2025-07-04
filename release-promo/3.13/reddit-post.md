**Title:** Cline 3.13 is Here: Toggleable `.clinerules`, `/new_task` Slash Command & Message Editing w/ Checkpoints!

Hey everyone,

Cline v3.13 just dropped, focusing on giving you more precise control over your AI development workflow and tackling common frustrations. Here are the highlights:

**Highlights:**

*   **Toggleable `.clinerules` Popover:** Stop manually juggling custom instructions! The new [popover UI](https://docs.cline.bot/prompting#managing-rules-with-the-toggleable-popover) (below the chat input) lets you easily see active global/local rules and toggle them on/off with a click. Switch Cline's "role" or context (like activating `memory-bank.md` or specific framework rules) instantly. Less friction, more precise guidance exactly when you need it. `[VIDEO: Cline Rules Popover Demo]`
    *   **Pro tip:** If you use a `.clinerule` to perform a specific workflow, ask Cline to make it better based on your feedback. This is "self-improving Cline"!

*   **`/new_task` Slash Command:** Quickly branch explorations or start a fresh task without losing context. Just type [`/new_task`](https://docs.cline.bot/exploring-clines-tools/new-task-tool#using-the-new_task-slash-command) in the chat input. It's a faster way to manage sessions, especially for keyboard-heavy users. More slash commands coming soon! `[VIDEO: Slash Command Demo]`

*   **Message Editing & Checkpoint Restore:** Fix typos in previous prompts or explore different paths without starting over using [Message Editing](https://docs.cline.bot/exploring-clines-tools/checkpoints#editing-messages). Hover over a message, click edit, and make changes. Crucially, you can also choose to **restore your entire workspace** (files, terminal state) back to that point using checkpoints. It's like infinite undo for your dev session, encouraging fearless experimentation. `[VIDEO: Message Editing & Checkpoints Demo]`

**Other Updates & Fixes:**

*   **New Model Support:** OpenAI `o3` & `4o-mini`, Azure DeepSeek, Google Gemini baseURL option. (Thanks @PeterDaveHello, @arafatkatze, @owengo, @olivierhub, @yt3trees!)
*   **Improved Search & Replace:** More robust diff editing, less falling back to full file overwrites. (Thanks @chi-cat!)
*   **Better Terminal Handling:** Improved `Ctrl+C` detection & large output chunking.
*   **MCP Image Responses:** Supported models can now get images from MCPs. (Thanks @rikaaa0928!)
*   **Fixes:** Vertex token tracking, xAI reasoning parsing. (Thanks @mzsima, @mrubens!)

We think these updates significantly improve workflow control and flexibility.

**Update to Cline 3.13 today** and let us know what you think!

*   **Blog Post:** [Link to blogs/cline-3-13-release.md when published]
*   **Docs:** https://docs.cline.bot
*   **Discord:** https://discord.gg/cline
