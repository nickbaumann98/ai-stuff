**v3.17.15** @everyone

*   **Provider Fixes:** Fixed an issue where LiteLLM would not respect the selected model when switching between Plan/Act modes (Thanks @sammcj!). We also removed a deprecated custom model encoding for the AWS Bedrock provider (Thanks @watany-dev!).
*   **UI & UX Fixes:** Chat input is no longer cleared when switching from Act to Plan mode without sending a message (Thanks @BarreiroT!). We also fixed timeline tooltips for followup messages (Thanks @char8x!).
*   **MCP Stability:** Fixed a bug that could cause MCP server names to display as "undefined" and fail tool invocations (Thanks @ramybenaroya!).
*   **Accessibility:** Task header buttons and the Plan/Act mode switch now properly report their state to screen readers (Thanks @yncat! 🙏).
*   **Environment:** Cline will no longer read development environment variables from the user's environment (Thanks @BarreiroT!).

Huge thanks to all our community contributors for this release! 🙏

If you have a chance to support us by [leaving a review](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev), we'd greatly appreciate it. Thank you!
