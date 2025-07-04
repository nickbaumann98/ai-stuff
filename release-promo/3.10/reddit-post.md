**Title:** Cline 3.10 Released: Connect to Local Chrome, Auto-Approve Commands, Drag & Drop + More!

Hey everyone,

Cline 3.10 is out, bringing some major workflow enhancements, especially a new way to interact with the web!

**Connect Cline to Your Local Chrome Browser**

This is the big one. You can now connect Cline directly to your running local Chrome browser instance via remote debugging (e.g., `localhost:9222`). This replaces the old sessionless browser and lets Cline operate within your *real* browser environment, using your existing logins, cookies, and session state.

What this unlocks:

*   **Seamless Debugging:** Point Cline at your local dev server and have it inspect elements, check network logs, etc., right in your active dev session. No more context switching.
*   **Session-Based Automation:** Let Cline leverage your logged-in sessions to interact with services like Gmail, Jira, internal tools, or even post to social media.
*   **Accessing Private Content:** Easily extract info or automate tasks on sites that require login, using your authenticated session.

This opens up possibilities for much more complex and stateful agentic workflows.

**Enable all commands (YOLO Mode)**

For full yolo mode, we've added the **"Enable all commands"** option. This means you now have the option to give Cline full auto-approve. Great for large refactors or complex command sequences, but **use with caution** and ensure you have backups/VC!

**New Task Tool**

We've added a "New Task" tool: Cline can create new tasks using context from the current conversation, allowing you to maintain task flow while opening a new context window.

Try using `.clinerules` to suggest that Cline "start a new task when the context window is 50% full."

**Streamlined Workflow Enhancements**

We've also added several other quality-of-life improvements:

*   **Easy MCP Server Management:** New modal in the chat area to quickly enable/disable MCP servers.
*   **Drag & Drop Context:** Drag files/folders onto the chat (hold **Shift** while dragging) to add context.
*   **CMD+' Shortcut:** Quickly add selected code/text to the Cline chat with `CMD+'` (Mac) / `Ctrl+'` (Win/Linux).
*   **Smarter Context Management:** Cline now automatically removes older, non-current document versions when context gets half full, improving performance and reducing looping.
*   **Prompt Caching:** For LiteLLM + Claude users, reducing redundant token use.
*   **Reduced System Prompt Size:** Dynamic loading of MCP docs makes the initial prompt smaller and more efficient.
*   **Fix:** MCP Auto-Approve toggle sync issue resolved.

**Get Started**

Update your Cline extension to 3.10 to check out these features. We think the local Chrome integration is a huge step forward and are excited to see what you build with it.

*   **Try it:** Connect to local Chrome and see what workflows you can automate.
*   **Feedback:** Join the discussion on our [Discord](<link-to-discord>) or here on [r/cline](<link-to-reddit-sub-r/cline>).
*   **Docs:** [https://docs.cline.bot](https://docs.cline.bot)

Happy coding!
