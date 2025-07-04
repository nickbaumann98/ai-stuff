Cline v3.17.14 is live.

This patch release adds more provider flexibility, new terminal controls, and a round of important stability fixes.

🧵

↓

First, we've expanded our provider support.

- You can now plug in Anthropic's Claude Code CLI tool as a provider.
- We've also added support for SAP AI Core, with access to both Claude and GPT models. (Thanks @schardosin!)

↓

Next, we've added more control over the terminal.

- Set a default terminal profile in settings to have Cline use your preferred shell. (Thanks valinha!)
- A new output size constraint helps prevent slowdowns from noisy commands.

↓

This release also includes key reliability improvements.

- We've fixed issues with checkpoint saving and task restoration for more accurate file tracking.
- The search/replace algorithm is now more robust, preventing an edge case that could cause file deletion.

↓

Check out the blog post for the full details.

↓

https://cline.bot/blog/cline-v3-17-14-new-provider-options-terminal-upgrades-and-core-fixes