Title: Cline v3.17.15: Community Fixes for Providers, UX, and Accessibility

---

Hey everyone, Nick from Cline here.

We just shipped v3.17.15, a patch release with a number of community-contributed fixes and improvements.

Here’s a quick rundown of what's new:

**Provider Reliability**

*   We fixed an issue with the LiteLLM provider to ensure it respects the selected model when switching between Plan and Act modes. (Thanks @sammcj!)
*   The AWS Bedrock provider was updated to remove a deprecated custom model encoding. (Thanks @watany-dev!)

**Core Experience & Stability**

*   The chat input will no longer be cleared when you switch between Plan/Act modes without sending a message. (Thanks @BarreiroT!)
*   We fixed a bug that could cause MCP server names to display as "undefined" and prevent tool/resource use. (Thanks @ramybenaroya!)
*   Timeline tooltips for followup messages have been fixed. (Thanks @char8x!)
*   Cline will no longer read development environment variables from the user's environment. (Thanks @BarreiroT!)

**Accessibility Improvements**

*   Task header buttons are now properly announced by screen readers.
*   The Plan/Act mode switch now correctly reports its state for screen readers.
*   A huge thank you to @yncat for these accessibility contributions!

As always, a massive thank you to all our community contributors who made this release possible. Let us know if you have any feedback!

-Nick 🫡
