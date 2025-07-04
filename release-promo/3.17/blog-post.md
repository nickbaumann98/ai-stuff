# 3.17: Global Workflows, UX Improvements, and More

Cline v3.17 brings several solid improvements to enhance your development workflow. The highlight is Global Workflows—a feature many of you have been requesting—along with a redesigned settings interface and expanded provider support.

## Global Workflows: Share Your Best Practices Across Projects

The standout feature in this release is global workflows. If you've built a workflow that works brilliantly in one project, you can now share it across all your workspaces.

[VIDEO: Global Workflows Demo]

Here's how it works:
- Global workflows live in `~/Documents/Cline/Workflows`
- Local workflows in `.cline/workflows/` take precedence
- No more copying workflow files between projects

This solves a real pain point. Many of you have crafted sophisticated workflows for specific tasks—API integration patterns, testing strategies, deployment sequences. Now these become part of your permanent toolkit, available wherever you need them.

## What's New

**Major Updates:**
- Global Workflows for sharing across projects
- Claude 4 support across all providers (Anthropic, AWS Bedrock, Vertex AI)
- Redesigned settings page with tabbed interface
- Nebius AI Studio integration (Thanks @Aktsvigun!)
- Enhanced Act mode prompts with hotkey suggestions

**Fixes & Improvements:**
- MCP server configuration fixes
- Requesty provider model listing
- Consolidated advanced settings
- AWS Bedrock environment variable handling improvements (Thanks @DaveFres!)
- Various stability improvements

## UX Refinements That Matter

Beyond the headline features, we've made several quality-of-life improvements:

**Redesigned Settings Page**: Split into tabs for easier navigation. When you're managing multiple API keys, model selections, and MCP configurations, organization matters. (Thanks to Yellow Bat @dlab-anton and the Roo Team for this contribution!)

[VISUAL: New Settings Interface]

**Smart Act Mode Prompts**: Cline now highlights and suggests hotkeys when the assistant prompts you to switch to Act mode. It's a small touch that makes the Plan/Act workflow more intuitive.

**MCP Server Fix**: Fixed a configuration bug that was preventing some MCP servers from initializing properly.

## What's Next

We're excited about the possibilities that Global Workflows open up. As more of you build and share sophisticated automation patterns, we're seeing a library of best practices emerge across the community. We're also exploring deeper integrations with providers like Nebius to give you even more flexibility in how you use Cline.

Ready to try the improvements? Update Cline in VS Code, Cursor, or Windsurf marketplace and let us know how the new features work for your workflow.

Join the conversation:
- Discord: https://discord.gg/cline
- Reddit: https://www.reddit.com/r/cline/
- Docs: https://docs.cline.bot

---

*PS: If you're building interesting workflows with the new global system, share them with the community. We're seeing some creative patterns emerge that are worth spreading.*
