---
title: ".clinerules: Version-Controlled, Shareable, and AI-Editable Instructions"
date: 2025-06-20
author: Nick Baumann
---

We've deprecated the "Custom Instructions" text box in Cline.

This isn't a big change for most of you - the majority of our users have already embraced the more powerful `.clinerules` system. But for those who were still using the old text box, it's time to make the switch.

**Why `.clinerules` Are Better**

The old Custom Instructions box was a single, static text field hidden in settings. It served its purpose, but `.clinerules` are simply better in every way:

*   **They're Toggleable:** This is huge. You can have multiple rule files and toggle them on/off as needed. Writing code? Activate your coding standards. Writing tests? Toggle on your testing guidelines. This flexibility means Cline adapts to your current task, not the other way around.
*   **They Live With Your Code:** Your AI guidance is right there in your project as `.md` files. They're version-controlled, PR-reviewable, and instantly available to anyone who clones your repo.
*   **They're Modular:** Break your instructions into focused files like `01-coding-style.md` or `react-patterns.md`. This makes rules easier to manage and reuse across projects.
*   **Cline Can Edit Them:** Because rules are just files, Cline can read, write, and edit them. Ask Cline to refine a rule based on your feedback, and it will. This creates a self-improving loop where your AI becomes more aligned with your needs.

**The Community Aspect**

One of the most exciting developments is the [cline/prompts](https://github.com/cline/prompts) repository on GitHub. It's a growing library of `.clinerules` and workflows from the community. Find rules that work for your projects, contribute your own, and help build collective knowledge about how to guide AI effectively.

**Getting Started with `.clinerules`**

If you haven't used `.clinerules` before (or even if you have), here's a quick refresher:

1.  **Create a Rule:** Click the `+` button in the Rules popover (below the chat input) to create a new Global or Workspace rule.
2.  **Toggle Rules On/Off:** Use the toggles in the popover to activate or deactivate specific rules as your needs change.
3.  **Organize Your Rules:** Consider creating a `.clinerules/` directory in your project for workspace-specific rules, and use the global rules for your personal preferences.
4.  **Explore the Community:** Check out the [cline/prompts](https://github.com/cline/prompts) repo for inspiration and reusable rules.

This isn't just a feature update. It's a philosophy shift. We believe AI instructions should be code - shareable, versionable, and collaborative. The old text box couldn't deliver on this vision. `.clinerules` can.
