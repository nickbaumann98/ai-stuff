---
title: "Cline v3.16: Unleash One-Shot Automation with Workflows, Plus UI & Stability Gains"
date: "2025-05-19" # Updated to today's date, can be adjusted
author: Nick Baumann
# featured_image: /content/images/2025/05/cline-v316-workflows-banner.png # Placeholder for a potential banner
---

Welcome to Cline v3.16! We're really excited about this release, especially a new feature that's already making a big difference for our own team: **Workflows**. We think it's going to help you supercharge your productivity and automate those repetitive tasks like never before. Let's dive in!

## → Workflows → Your Personal Automation Powerhouse

You know those repetitive sequences you find yourself doing all the time? Setting up a new project module, running through a pre-commit checklist, or even the detailed steps for a PR review. It's often the same clicks, the same commands. What if you could just tell Cline, "Handle my usual PR review prep for this one," and watch it go?

That's exactly what **Workflows** are designed for.

[VIDEO: Watch Cline automate a PR Review using Workflows! (approx. 30-60 seconds) This demo shows the "one-shot" power of defining and executing a complex task.]

Workflows are your personal automation scripts, living right within your project. Accessed via a new "Workflows" tab in the Cline interface, you can easily create `.md` files that define a series of steps for Cline to follow. The real power comes from how you structure these files: you can leverage Cline's built-in tools (like `read_file` or `ask_followup_question`), use command-line tools you already have installed (like `gh` or `docker`), reference external MCP tool calls, and chain multiple actions together in a specific sequence. This allows you to compose various capabilities, much like building with LEGO blocks, into a seamless, automated process.

As one of our own developers put it: *"This is probably going to save me thousands of hours of time automating repetitive tasks that I normally have to do manually. Now I could just tell Cline to do them... Your imagination is the limit!"*

[VISUAL: Screenshot of the new "Workflows" tab in the Cline UI, perhaps showing a list of example workflow files like "pr-review.md" or "extension-release.md".]

**So, what's the big deal? For us, it boils down to a few key things:**
*   **True "One-Shot" Power:** Imagine kicking off a whole series of complex steps with just one simple `/[workflow-name.md]` command (using the exact filename). That's the core idea.
*   **It's More Than Just Scripting:** These aren't just basic scripts. Workflows tap into Cline's ability to understand what you're doing, use its tools, and work with your code, making the automation much smarter.
*   **Real Time Savings:** We're talking about tasks that used to take minutes, sometimes longer, now getting done in moments. Those savings add up fast.
*   **Doing it Right, Every Time:** By defining your process in a workflow, you get consistency. No more missed steps or variations that lead to errors.
*   **Tailored to Your Projects:** Workflows live in your project's `.clinerules/workflows/` folder, so they're version-controlled and specific to what that project needs.

A prime example we're already using internally (and the one featured in our video demo!) is a **PR Review workflow**. This workflow, detailed in our new documentation, uses the `gh` command-line tool to pull PR details, examine diffs, check surrounding files, analyze changes, and even ask for confirmation to approve the PR with a drafted comment. It transforms a manual, multi-step operation into a single command, giving you everything needed for an informed decision. The potential is massive, and we can't wait to see what *you* build.

You can dive deeper into creating and using workflows with our **[Workflows Documentation](https://docs.cline.bot/features/slash-commands/workflows)**. You'll find more details there, including the `pr-review.md` example. For now, start thinking about those repetitive tasks you'd love to automate -- Workflows are here to help.

## Key Enhancements & Fixes in v3.16

While Workflows steal the spotlight, this release is packed with other significant improvements and stability gains, combining updates from both v3.16.0:

*   **New Workflow Feature:** Create and manage workflow files callable via slash commands (The star of the show!).
*   **Collapsible Recent Task List:** Easily hide your task history when sharing your screen. (Thanks to community contributor **@cosmix**!)
*   **Global Endpoint for Vertex AI:** Higher availability and fewer 429 errors for Vertex AI users. (Thanks **@soniqua**!)
*   **Improved Auto-Approve Functionality:**
    *   **Enable Auto-Approve Toggle:** Easily turn auto-approve on/off without losing action settings.
    *   **UI Styling Update:** Conserved space in the auto-approve menu.
    *   **Quick Actions Fix:** Resolved issues with quick actions in auto-approve settings.
*   **Enhanced Gemini Model Interaction:**
    *   **Improved Retry Handling:** Better UI feedback and progress indication for Gemini API request retries.
*   **New User Experience:** Special components and guidance to help new users get started smoothly.
*   **Settings Organization:** VSCode Advanced settings migrated to the Settings Webview for a cleaner experience.
*   **Memory Leak Fix:** Addressed a memory leak that could occur during long sessions.
*   **Eternal Loading State Fix:** Resolved issues when the last message was a checkpoint. (Thanks **@BarreiroT**!)

## Get Rolling with v3.16

Ready to unleash one-shot automation with Workflows and benefit from all the latest improvements?

*   **Update now** via the VS Code Marketplace, Cursor, or Windsurf!
*   Read the full [**Changelog**](https://github.com/cline/cline/blob/main/CHANGELOG.md)
*   Join the discussion on [**Discord**](https://discord.gg/cline)
*   Check out the new [**Workflows Documentation**](https://docs.cline.bot/features/slash-commands/workflows) and our general [**Docs**](https://docs.cline.bot).
*   If Cline is helping you build faster, please consider [**leaving a review**](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev). It makes a huge difference!

Happy Automating!

-Nick
