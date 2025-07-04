# Unlocking Persistent Memory: How Cline's `new_task` Tool Eliminates Context Window Limitations

Context windows have been both the power and limitation of AI coding assistants. They enable the contextual understanding that makes tools like Cline so useful, but their finite nature has always imposed constraints on complex, long-running tasks.

With Cline's latest features, we've created a solution that fundamentally changes how developers can work with AI assistants on complex projects.

## The Context Window Problem

We implemented the context progress bar to make it visual when users should start new tasks. This is because after exceeding 50% of the context window, performance can dip, Cline might "forget" earlier parts of a conversation, and restarting means tedious re-explanation.

While larger context windows help (i.e. Gemini 2.5 Pro & GPT-4.1's 1m context window), they aren't a complete solution. What if Cline could proactively manage its own context *before* hitting limits?

## A True "1 + 1 = 3" Solution

Cline now offers the building blocks to create exactly this kind of workflow, enabling a form of persistent memory for complex, long-running tasks. It's not just a single feature, but a powerful combination of capabilities that creates something greater than the sum of its parts:

**1. Context Window Awareness:** Cline internally tracks its context window usage (you can see this percentage in `environment_details`). It knows when it's approaching limits where performance might degrade (often noticeable past ~50% usage for many models).

**2. The `new_task` Tool:** This internal tool allows Cline (with your approval) to cleanly end the current session and immediately start a new one. Crucially, it can preload this new session with specific, structured context – summaries, file states, next steps, etc.

**3. `.clinerules` for Automation:** This is where the magic happens. You can define rules in `.clinerules` that tell Cline *when* to propose a handoff (e.g., "if context usage > 50%") and exactly *what* information to package into the `<context>` block of the `new_task` tool.

## How It Works in Practice

The workflow we've designed is both powerful and elegant in its simplicity:

1. **Monitor:** Cline monitors context usage as defined in your `.clinerules`.
2. **Trigger:** When a threshold (e.g., 50%) is hit, Cline finishes its current step.
3. **Propose:** Cline uses `ask_followup_question` to suggest creating a new task, showing the structured context it plans to carry over (based on your rules).
4. **Handoff:** If you approve, Cline uses `new_task`, ending the current session and starting a new one instantly, preloaded with the precise context needed to continue.

## Beyond Context Limits: The Real Benefits

By combining these elements, you create a workflow where Cline intelligently manages its own context *before* performance degrades or information is lost. No more manual resets just because the context window is full, and less time spent re-explaining the project state. 

For complex tasks spanning multiple sessions, it provides a much smoother experience, feeling closer to working with an agent that has persistent memory. This allows you to focus on the coding task, letting the `.clinerules` handle the context management automatically in the background.

## Looking Forward

The `new_task` tool opens up a realm of possibilities beyond just context management. It enables structured workflows for complex projects, better task decomposition, and more predictable AI assistance. The rule-driven nature of the system means it's highly customizable to your specific development patterns and needs.

We're just beginning to explore what's possible with this paradigm of AI-assisted development. From automated context summarization to intelligent handoffs between specialized agents, this foundation serves as a springboard for future innovations.

## Try It Yourself

The new `new_task` tool is now available to all Cline users. We've provided comprehensive documentation to help you get started with building workflows that overcome context limitations.

* [new_task tool docs](https://docs.cline.bot/exploring-clines-tools/new-task-tool)
* [Visual explanation](https://x.com/cline/status/1912279346338996425)

How have you experimented with the `new_task` tool & `.clinerules`? We'd love to hear about your experiences and ideas in the comments below.
