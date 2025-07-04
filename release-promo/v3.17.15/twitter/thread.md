Cline v3.17.15 is live.

This patch release is packed with community-led fixes that improve provider stability, core UX, and accessibility.

🧵

[VISUAL: A summary graphic of the key fixes in v3.17.15]

---

First, we've shipped several key provider fixes.

- The LiteLLM provider now correctly respects the selected model when switching between Plan/Act modes. (Thanks @sammcj!)
- The AWS Bedrock provider has been updated to remove a deprecated dependency. (Thanks @watany-dev!)

---

Next, we've improved the core experience and fixed some pesky bugs.

- Chat input is no longer cleared when switching between Plan/Act modes. (Thanks @BarreiroT!)
- A bug causing MCP server names to show as "undefined" has been squashed. (Thanks @ramybenaroya!)

---

This release also includes important accessibility improvements, ensuring task headers and the Plan/Act mode switch are now properly announced by screen readers. (Thanks @yncat! 🙏)

---

As always, a huge thank you to all the community members who contributed to this release.

Check out the full changelog for more details. 👇

https://github.com/cline/cline/blob/main/CHANGELOG.md
