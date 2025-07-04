**Title: Cline v3.17.14: New Provider Options (Claude Code, SAP), Terminal Upgrades, and Core Fixes**

Hey everyone, Nick from Cline here.

We just shipped a patch release, v3.17.14, with a focus on expanding provider flexibility and improving the core developer experience.

Here’s a quick rundown:

**New Provider Integrations**

*   **Claude Code:** You can now use Anthropic's Claude Code CLI tool as a provider in Cline. If you have it installed locally, you can plug it right in and use your Claude Max Plan.
*   **SAP AI Core:** We've also added support for SAP AI Core, allowing connections to both Claude and GPT models through the service. (Thanks @schardosin!)

**Terminal Experience Upgrades**

*   You can now set a **default terminal profile** in settings to specify which terminal Cline should use. This should help with some of the ongoing shell integration issues. (Thanks @valinha!)
*   We added a **terminal output size constraint** setting to prevent Cline from getting bogged down by commands with massive outputs.

**Core Improvements & Fixes**

We also shipped a number of reliability improvements:

*   **Better Stability:** We fixed issues with task restoration and checkpoint saving for more accurate file tracking, and made our search/replace algorithm more lenient to prevent an edge case that could delete files.
*   **AWS Bedrock Update:** The Bedrock provider now uses the standard AWS SDK, removing a deprecated dependency. (Thanks @watany-dev!)
*   **Other Fixes:** We also improved the `list_files` tool, MCP Rich Display settings persistence (thanks @Vl4diC0de!), and refactored some UI components (thanks @shouhanzen!).

As always, you can grab the update from the VS Code or Cursor marketplace. Let us know if you have any feedback.

- Nick 🫡
