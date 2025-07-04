v3.13.0 @everyone

*   **`.clinerules` Popover:** Easily add, enable & disable workspace/global rule files via the new UI under the chat input for quick context switching.
*   **Slash Command:** Type `/new_task` to quickly create a new task while preserving context.
*   **Message Editing & Restore:** Edit past messages and optionally restore your workspace back to that point using checkpoints.
*   **Send Message with Option:** You can now type a message while also selecting a suggested option from Cline.
*   **Jump to Chat Input:** New command palette action (assignable to keybinding) to focus the Cline chat input from anywhere in VS Code.
*   **Model Support:** Added OpenAI `o3` & `4o-mini` (Thanks @PeterDaveHello, @arafatkatze!), Azure DeepSeek (Thanks @yt3trees!), and Google Gemini `baseURL` option (Thanks @owengo, @olivierhub!).
*   **MCP Image Responses:** Models supporting image input can now receive images from MCP servers (Thanks @rikaaa0928!).
*   **Improved Search/Replace:** More robust diff editing, less likely to fall back to full file writes (Thanks @chi-cat!).
*   **Terminal Improvements:** Better detection of `Ctrl+C` termination and chunking for large outputs to improve performance.
*   **Fixes:** Addressed issues with Vertex token tracking (Thanks @mzsima!) and xAI reasoning parsing (Thanks @mrubens!).

Huge thanks to all community contributors! 🙏

**Update now** via VS Code/Cursor Marketplace!

Read the full details: [Link to blogs/cline-3-13-release.md when published]
Docs: https://docs.cline.bot

If you have a chance to support us by [leaving a review](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev), we'd greatly appreciate it. Thank you!
