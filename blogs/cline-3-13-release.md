# Cline 3.13: Toggleable .clinerules, Slash Commands & Previous Message Editing

Tired of manually managing context instructions for different tasks? Wish you could quickly branch explorations or fix a flawed prompt without starting over? Cline 3.13 tackles these workflow frustrations head-on. We're delivering precise control over your AI development process with three key updates: Toggleable `.clinerules` for effortless context switching, quick `/new_task` Slash Commands for session management, and powerful Message Editing with Checkpoint Restore for fearless exploration. Here’s why these updates will make your life easier and how to start using them today.

**Stop Juggling Context: Toggle `.clinerules` On Demand**

You asked for more control over how Cline uses custom instructions, and v3.13 delivers. Forget manually editing prompts or managing complex configurations. The new [`.clinerules` popover](https://docs.cline.bot/prompting#managing-rules-with-the-toggleable-popover), right below the chat input, lets you treat your instruction files like modular roles you can instantly switch between. Need Cline to remember project specifics? Toggle on your `memory-bank.md`. Working on the UI? Activate your `react-best-practices.md`. This popover shows active global and local rules and lets you enable or disable them with a click. Add new rules easily and activate them *only* when relevant. Why care? It means less friction and more precise AI guidance exactly when you need it, making Cline adapt seamlessly to your workflow.

**Slash Commands: Your Keyboard Shortcut to Productivity**

We're always looking for ways to accelerate your workflow. Cline 3.13 introduces Slash Commands, starting with a quick way to manage your sessions. Simply type [`/new_task`](https://docs.cline.bot/exploring-clines-tools/new-task-tool#using-the-new_task-slash-command) in the chat input, and Cline will initiate the process of creating a new task, preserving the context from your current session – perfect for branching explorations or starting fresh without losing your place. This is just the beginning for Slash Commands; expect more quick actions in the future! Combined with the new "Jump to Cline Chat Input" command (accessible via the command palette and assignable to a keybinding), keyboard warriors can navigate and interact with Cline faster than ever.

**Edit the Past, Reshape the Future: Message Editing & Checkpoints**

Ever wished you could tweak a previous prompt without retyping everything? Or explore a different coding path without starting a whole new chat? Now you can. Cline 3.13 introduces the ability to [edit your previous messages](https://docs.cline.bot/exploring-clines-tools/checkpoints#editing-messages). Simply hover over a message and click the edit icon. But it's more than just fixing typos. When you edit a message, Cline leverages its powerful checkpoint system, offering you the option to **restore your workspace** back to the state it was in *before* that message was sent. It's like having infinite undo for your entire development session. Made a wrong turn? Realized a different approach would be better? Just edit the relevant message, restore the checkpoint, and proceed down the new path. This fundamentally changes how you can interact with Cline, encouraging experimentation and making it trivial to backtrack and refine your approach.

**And More...**

Beyond these headline features, Cline 3.13 includes several other valuable updates:

*   **New Model Support:** We've added support for OpenAI's `o3` and `4o-mini`, Azure's DeepSeek model, and enabled baseURL configuration for Google Gemini. (Thanks @PeterDaveHello, @arafatkatze, @owengo, @olivierhub, @yt3trees!)
*   **Improved Search & Replace:** We've refactored the logic for applying diff edits, making it more robust and less likely to fall back to overwriting the entire file when an LLM provides slightly imperfect instructions. This means more reliable, targeted code changes. (Thanks @chi-cat!)
*   **Enhanced Terminal Handling:** Better detection of `Ctrl+C` termination and chunking for large outputs improves performance and reliability when working with terminal commands.
*   **MCP Image Responses:** Models that support it can now receive image responses from MCP servers. (Thanks @rikaaa0928!)
*   **Bug Fixes:** Addressed issues with Vertex token tracking and xAI reasoning parsing. (Thanks @mzsima, @mrubens!)

**Take Control Today**

Cline 3.13 puts more power and precision directly into your hands. From modular AI guidance with toggleable rules to rapid actions via Slash Commands and the freedom to reshape your session history with message editing – these features are designed to make your development workflow smoother, faster, and more adaptable.

**Update to Cline 3.13 today** and experience the difference. Let us know what you think!

*   Explore the features in our [Docs](https://docs.cline.bot)
*   Join the discussion on [Reddit](https://www.reddit.com/r/cline/)
*   Chat with the community on [Discord](https://discord.gg/cline)
