**Title: How to use your Claude Max subscription in Cline**

Hey everyone,

Seeing lots of questions regarding how to setup Claude Code in Cline and take advantage of your Claude Max plan ($200/month for Claude models). Here's how you can use the Claude Code provider in Cline:

1.  **Install Claude Code:** Make sure you have Claude Code installed and authenticated.
2.  **Configure in Cline:**
    *   Go to `Settings` > `API Configuration`.
    *   Select `Claude Code` from the provider dropdown.
    *   Set the path to the CLI (usually just `claude` if it's in your system's PATH).

If `claude` doesn't work, you can enter your full path -- find it by running one of the following commands (depending on your machine):

**macOS / Linux:** which claude
**Windows (Command Prompt):** where claude
**Windows (PowerShell):** Get-Command claude

**How it works:**

When you select Claude Code as your provider, here's what happens under the hood:

1. You send a message in Cline's interface
2. Cline spawns a subprocess running the Claude Code CLI (`claude -p --output-format stream-json`)
3. Your message and conversation history are passed to Claude Code as JSON arguments
4. Claude Code connects to Anthropic's API and processes your request
5. Responses stream back as JSON which Cline parses and displays in your chat
6. The subprocess terminates after each response (Cline manages the ongoing conversation)

In essence, Cline wraps the Claude Code CLI -- every message triggers a new `claude` command. Claude Code's built-in tools (file reading, bash commands, etc.) are disabled to prevent conflicts, with all actual tool execution handled by Cline's own tools. The AI reasoning comes from Claude Code, but the system interactions come from Cline. The main user-visible difference is that responses don't stream character-by-character - Claude Code processes the full request before sending back complete responses.

Here's the link to the full documentation with more details:
https://docs.cline.bot/providers/claude-code
