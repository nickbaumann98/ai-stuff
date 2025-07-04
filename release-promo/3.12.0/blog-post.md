# Cline v3.12: Faster Diff Edits, Model Favorites, and More

We're excited to announce the release of Cline v3.12, packed with diff edit improvements, model favorites, new auto-approve options, and more.

Let's dive into the highlights:

## Faster Diff Application [VISUAL: Diff Edit Animation Comparison]

Applying code changes suggested by Cline is now significantly faster, especially in large files. v3.12 boosts diff edit performance for a smoother, more responsive experience, letting you iterate faster.

We've also added an indicator in the chat view showing the number of edits being made for better transparency.

## Quick Access: Model Favorites [VISUAL: Favorite Model Toggle]

Switching LLMs is easier with Model Favorites. Using Cline or OpenRouter providers? Mark models as favorites in the dropdown. They'll appear at the top for quick access, saving scroll time. Personalize your workflow and keep go-to models a click away.

## Enhanced Control: New Auto-Approve Options

Cline v3.12 adds granularity to auto-approve settings. You can now disable Cline's ability to automatically read/edit files *outside* your workspace directory. This adds safety, ensuring Cline operates within defined project boundaries unless explicitly approved elsewhere. Find these toggles in settings.

## Expanding Model Support: Grok 3 Mini Integration

Cline now supports streaming responses and the "reasoning effort" option for xAI's Grok 3 Mini model, allowing for more interactive and potentially higher-quality outputs from this provider.

## Quality of Life & Bug Fixes

This release also includes several important improvements and fixes:

*   **Easier MCP Management:** A new settings button has been added to the MCP popover, providing quick access to modify your installed MCP server configurations.
*   **Ollama Enhancements:** The Ollama provider now includes a retry mechanism for transient network issues, better timeout handling, and clearer error messages for a more robust local model experience (big thanks to community member `suvarchal` for the contribution!).
*   **Browser Tool Fix:** Resolved a critical bug where actions performed by the browser tool weren't displaying their results correctly in the chat.
*   **Checkpoint Fixes:** Addressed issues with the new checkpoint popover hiding too quickly and a bug causing duplicate checkpoints.

## Get Started with v3.12

Cline v3.12 focuses on refining the core experience – making edits faster, model selection quicker, and providing more control, all while squashing important bugs.

**Ready to upgrade?** Update Cline through the VS Code Marketplace or download the latest version.

Check out the full [changelog](https://github.com/cline/cline/blob/main/CHANGELOG.md) for all the details.

We're constantly working to improve Cline based on your feedback. Join the conversation and share your thoughts on our [Discord](https://discord.gg/cline) or [Reddit](https://www.reddit.com/r/cline/) community!
