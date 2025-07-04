**Title:** Cline v3.16 Released: Introducing Workflows for One-Shot Automation!

---

Hey everyone,

Cline v3.16 is out! We've been experimenting with workflows A LOT lately, and now we're excited to share them with you!

Workflows are your personal automation scripts, living right within your project. Accessed via a new "Workflows" tab, you can easily create `.md` files that define a series of steps for Cline to follow. Think of it like building with LEGO blocks: you can compose CLI commands, existing Cline tools (like `read_file` or `ask_followup_question`), and even powerful MCP tools into a seamless, automated process. This means true "one-shot" power – kick off complex multi-step tasks with a single `/[workflow-name.md]` command (using the exact filename). It's more than just scripting; Workflows tap into Cline's ability to understand context and interact with your code, leading to real time savings and consistent, reliable execution. Plus, they're stored in your project's `.clinerules/workflows/` folder, so they're version-controlled and tailored to each project's specific needs.

As one of our own developers (Nik Pash) put it: *"This is probably going to save me thousands of hours of time... Your imagination is the limit!"*

We're incredibly excited about the potential here and can't wait to see what you automate!

Here's what else we've got in this release:

*   **Collapsible Recent Task List:** Easily hide your task history when sharing your screen. (Thanks cosmix!)
*   **Enable Auto-Approve Toggle:** Conveniently turn auto-approve on/off without losing your action settings.
*   **Improved Gemini Retry Handling:** Better UI feedback and progress indication for Gemini API requests.
*   **Global Endpoint for Vertex AI:** Higher availability and fewer 429 errors for Vertex AI users. (Thanks soniqua!)
*   **Settings Organization:** VSCode Advanced settings have been migrated to the Settings Webview for a cleaner experience.
*   **Memory Leak Fix:** Addressed a memory leak that could occur during long sessions.
*   **Eternal Loading State Fix:** Resolved issues when the last message was a checkpoint. (Thanks BarreiroT!)
*   **Auto-Approve UI Enhancements:** Including fixes for quick actions and more concise menu styling for better usability.

Can't wait for you all to give workflows a shot! We'll be adding more examples in the coming days -- please share what you learn with the rest of the Cline community!

[**Workflows Documentation**](https://docs.cline.bot/features/slash-commands/workflows)!
Read the full details in our [**latest blog post**](https://cline.bot/blog/cline-v3-16-one-shot-automation-with-workflows-plus-ui-stability-gains)!
Check out the full [**Changelog**](https://github.com/cline/cline/blob/main/CHANGELOG.md) for all the details.

Update now via the VS Code Marketplace, Cursor, or Windsurf!

Let us know what you think here or on [**Discord**](https://discord.gg/cline)!

Happy automating!

-Nick
