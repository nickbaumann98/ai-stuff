---
title: "How to Use Your Claude Max Subscription in Cline"
date: 2025-06-24
description: "A guide on connecting your Claude Max subscription to Cline to save on token costs by using the Claude Code provider."
---

If you're a Cline user with a Claude Max subscription, you can connect your account to save on token costs. Instead of paying per token via an API key, the Claude Code provider lets you leverage your existing subscription for all your development tasks in Cline.

<figure>
  <video src="https://storage.googleapis.com/cline_public_images/docs/assets/claude-code-use-opus.mp4" autoplay loop muted playsinline></video>
</figure>

### Setup

Getting started is straightforward.

1.  **Install Claude Code**: First, follow Anthropic's [official setup guide](https://docs.anthropic.com/en/docs/claude-code/setup) to install and authenticate their CLI.

2.  **Configure in Cline**:
    - Navigate to **Settings** > **API Configuration**.
    - Select **Claude Code** from the **API Provider** dropdown.
    - Set the path to your Claude CLI executable. This is usually just `claude` if it's in your system's PATH.

<figure>
  <video src="https://storage.googleapis.com/cline_public_images/docs/assets/claude-code-setup.mp4" autoplay loop muted playsinline></video>
</figure>

To find your Claude Code path, you can use one of the following commands in your terminal:

*   **macOS / Linux**: `which claude`
*   **Windows (Command Prompt)**: `where claude`
*   **Windows (PowerShell)**: `Get-Command claude`

### How It Works

When you select Claude Code as your provider, Cline intelligently wraps the Claude Code CLI. For every message you send, Cline spawns a `claude` command in the background, passing your conversation history securely.

The AI reasoning comes from Claude, while Cline handles all the tool execution -- like running terminal commands or editing files. This integration means you get the power of Claude's models combined with the safety and control of Cline's human-in-the-loop workflow.

The main user-visible difference is that responses don't stream character-by-character. Claude Code processes the full request before sending back the complete response.

### Supported Models

The provider supports all models available through the CLI, including:

*   `claude-sonnet-4-20250514`
*   `claude-opus-4-20250514`
*   `claude-3-7-sonnet-20250219`
*   `claude-3-5-sonnet-20241022`
*   `claude-3-5-haiku-20241022`

### Limitations

There are a couple of limitations to be aware of with this provider:

*   **No image support**: Images in your messages will be converted to text placeholders.
*   **No prompt caching**: This feature is not available with Claude Code.

### Troubleshooting

If you run into any issues, here are a few things to check:

1.  **Verify Authentication**: Make sure you're properly logged into Claude Code with your subscription account.
2.  **Check Path**: Ensure the Claude CLI path in Cline's settings is correct.
3.  **Get Help**: We're still working on improving this integration. For issues, please [submit an issue on our GitHub](https://github.com/cline/cline/issues) or ask in our [Discord](https://discord.gg/cline).

### More Information

When using your Claude subscription, usage will still appear in Cline's billing interface as normal, but Max subscribers will see **$0.00 costs**, since no additional charges apply.

For more details, you can always refer to Anthropic's official documentation:

*   [Claude Code Setup Guide](https://docs.anthropic.com/en/docs/claude-code/setup)
*   [Using Claude Code with Pro/Max Plans](https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-pro-or-max-plan)
