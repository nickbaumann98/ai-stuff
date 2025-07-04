Cline 3.10 is live. The headline feature: connect Cline directly to your running local Chrome browser instance via remote debugging.

This moves beyond sessionless browsing, letting Cline operate agentically within your *real* browser. 🧵
`[VIDEO: Release Overview]`



What does the new local Chrome connection enable?

Debug web apps faster: Cline inspects elements/logs in your *active* Chrome session (`localhost:9222`), helping fix stateful UI bugs without context switching.
`[VIDEO: Chrome Use Case 1 - Debugging]`


Automate stateful tasks: Cline leverages your logins to interact with web apps (email, PM tools, etc.) using your active session.
`[VIDEO: Chrome Use Case 2 - Agentic Tasks]`


Access private content: Cline summarizes info from logged-in sites or dashboards using your authenticated session, avoiding manual copy-paste.
`[VIDEO: Chrome Use Case 3 - Private Content Extraction]`



Also new in 3.10: Need full autonomy? Enable YOLO Mode ("Enable all commands").

It auto-approves *all* actions (edits, commands) for max speed on complex tasks. (Use carefully!)
`[VIDEO: YOLO Mode]`



We've also added workflow enhancements for speed & ease:

- Drag & Drop Context: Drag files/folders onto chat (hold Shift) for instant context building.
- MCP Modal: Quickly enable/disable MCP servers directly from the chat input.
- New Task Tool: Cline can create new tasks autonomously - great for sub-tasking or a clean slate.
- CMD+' Shortcut: Add selected code/text to chat instantly (`CMD+'` / `Ctrl+'`).
`[VIDEO: Drag and Drop]`
`[VIDEO: MCP Modal]`



And under-the-hood improvements for efficiency & reliability:

Smarter context handling: Cline now auto-removes older doc versions when context fills, improving performance & reducing looping on long tasks.

Plus: Prompt Caching (LiteLLM+Claude), smaller system prompts (dynamic MCP docs), and MCP auto-approve sync fixes boost performance.



Cline 3.10 represents a significant step, especially with the local Chrome integration opening up new stateful workflow possibilities.

Update your extension to explore the new features.

Read the full breakdown: <link-to-blog-post>
Docs: https://docs.cline.bot
