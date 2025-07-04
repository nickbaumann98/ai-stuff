# Cline v3.13.3 Release: /smol Context Compression, Gemini Caching (Cline/OpenRouter), MCP Download Counts

Hey everyone! We just shipped v3.13.3 with some useful updates focused on managing context, reducing costs, and improving usability.

Here's what's new:

*   **`/smol` Slash Command 🤏:** Got a super long Cline conversation going but aren't ready to start a new task? Use the new `/smol` command (also works with `/compact`) to compress the chat history *within your current task*. Cline summarizes the conversation, which helps reduce token usage on subsequent turns and lets you keep your flow going longer. Think of it as in-place compression for your current session. [VIDEO: /compact command demo]
*   **`/smol` vs. `/new_task` Explained:** Here's what to know about when to use which!
    *   Use `/smol` when you want to continue the *same task* but the history is getting long/expensive (like during extended debugging). It shrinks the current context.
    *   Use `/new_task` when you've finished a distinct phase of work and want to start a *fresh, separate task*, carrying over only essential context. It's for moving cleanly between workstreams.
*   **Gemini 2.5 Pro Prompt Caching:** If you're using Gemini 2.5 Pro through the built-in Cline provider or OpenRouter, you should see significantly lower costs. We've added prompt caching, so repeated parts of the prompt aren't resent constantly. Users have reported savings up to 50% in some cases with the Gemini provider!
*   **MCP Download Counts:** Want to see which MCP servers are popular in the community? The Marketplace now shows download counts, making it easier to discover useful tools. [VISUAL: MCP Marketplace with Download Counts]
*   **UI Tooltips:** A small quality-of-life update -- we added tooltips to the bottom action bar icons to make navigation clearer. [VISUAL: Screenshot showing tooltips on bottom bar]

Update to v3.13.3 via the VS Code Marketplace to check out these improvements.

Let us know what you think or what features you'd like to see next!

Docs: https://docs.cline.bot
Discord: https://discord.gg/cline
