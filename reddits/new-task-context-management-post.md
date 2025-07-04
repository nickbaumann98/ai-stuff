We implemented the context progress bar to make it visual when users should start new tasks. This is because after exceeding 50% of the context window, performance can dip, Cline might "forget" earlier parts of a conversation, and restarting means tedious re-explanation.

While larger context windows help (i.e. Gemini 2.5 Pro & GPT-4.1's 1m context window), they aren't a complete solution. What if Cline could proactively manage its own context *before* hitting limits?

Cline now offers the building blocks to create exactly this kind of workflow, enabling a form of persistent memory for complex, long-running tasks. Here's how it works:

**1. Context Window Awareness:** Cline internally tracks its context window usage (you can see this percentage in `environment_details`). It knows when it's approaching limits where performance might degrade (often noticeable past \~50% usage for many models).

**2. The** `new_task` **Tool:** This internal tool allows Cline (with your approval) to cleanly end the current session and immediately start a new one. Crucially, it can preload this new session with specific, structured context – summaries, file states, next steps, etc.

**3.** `.clinerules` **for Automation:** This is where the magic happens. You can define rules in `.clinerules` that tell Cline *when* to propose a handoff (e.g., "if context usage > 50%") and exactly *what* information to package into the `<context>` block of the `new_task` tool.

**The Workflow in Action:**

1. **Monitor:** Cline monitors context usage as defined in your `.clinerules`.
2. **Trigger:** When a threshold (e.g., 50%) is hit, Cline finishes its current step.
3. **Propose:** Cline uses `ask_followup_question` to suggest creating a new task, showing the structured context it plans to carry over (based on your rules).
4. **Handoff:** If you approve, Cline uses `new_task`, ending the current session and starting a new one instantly, preloaded with the precise context needed to continue.

**The Outcome:**

By combining these elements, you create a workflow where Cline intelligently manages its own context *before* performance degrades or information is lost. No more manual resets just because the context window is full, and less time spent re-explaining the project state. For complex tasks spanning multiple sessions, it provides a much smoother experience, feeling closer to working with an agent that has persistent memory.

This allows you to focus on the coding task, letting the `.clinerules` handle the context management automatically in the background.

The new\_task tool opens up a ton of possibilities -- how have you experimented with the new\_task tool & .clinerules?

[**new\_task tool docs**](https://docs.cline.bot/exploring-clines-tools/new-task-tool)

[visual explanation](https://x.com/cline/status/1912279346338996425)