**v3.10.0 @everyone**

*   **Browser Tool Upgrades:** Use your local Chrome browser for session-based browsing, enabling debugging and productivity workflows tied to your actual (logged in) browser state!
*   **Auto-Approve Commands:** New 'Execute all commands' option to automatically approve ALL commands (use at your own risk!)
*   **Easily Toggle MCP's:** New modal in the chat area to easily enable/disable MCP servers.
*   **Smarter Context Management:** When hitting context window limits, old file contents are removed first. This preserves narrative integrity and prevents Cline from getting stuck in loops.
*   **Drag & Drop Context:** Drag and drop files/folders into chat by holding Shift while dragging it into the chat field.
*   **Reduced System Prompt:** Reduces system prompt token size by 30% by dynamically loading MCP documentation only when needed.
*   **Fix:** Fix MCP auto approve toggle issues being out of sync with settings. (Also includes prompt caching fix for LiteLLM+Claude).