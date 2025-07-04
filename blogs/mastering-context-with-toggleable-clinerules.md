As Product Marketing Manager at Cline, I often experiment with ways to fine-tune Cline's behavior for different tasks. For a while, I relied on a system of .clinerules/ and clinerules-bank/ folders, manually dragging rule files back and forth to activate different instruction sets. Honestly? It was kind of annoying – difficult to keep track of which rules were active, easy to forget to switch them, and just generally cumbersome. But I did get tremendous value from the "modular" nature of these .clinerules.
That's why the new toggleable .clinerules UI introduced in Cline v3.13 is such a welcome improvement. It replaces that manual file management with simple clicks, offering a much smoother way to control Cline's instructions on the fly.
Let's look at how this works and the practical benefits it brings to your workflow.
Global vs. Workspace Rules
Let's quickly recap the two types of rules Cline uses, both now easily managed via the popover:
Global Rules: Stored in a central Cline rules folder on your system (like ~/Documents/Cline/Rules on macOS/Linux, or similar on Windows), these rules are available across all your projects. Think of them for your universal coding style, preferred persona, or general instructions you always want active unless specifically turned off.
Workspace Rules: Located in a .clinerules/ directory within your current project's root, these are specific to that codebase. Use them for team standards, project-specific context, or guidelines relevant only to that repository.
The key thing to remember is that the content of any rule file you toggle 'on' (global or workspace) gets appended directly to Cline's system prompt for that session. This isn't just passive context; it actively shapes Cline's core reasoning and how it executes your requests..clinerules (i.e. "Custom Instructions") are appended to the bottom of Cline's system prompt when toggled "on"


The v3.13 Popover: Your New Control Panel
The manual process I described earlier – dragging files around – is now history. The v3.13 .clinerules popover (right below the chat input) is your central hub:
See What's Active: Instantly view all available Global and Workspace rules and their current on/off status.
Add Rules Easily: Use the '+' buttons to create new, blank rule files (.md) in either the global or workspace scope. Cline automatically handles creating the necessary folders (~/Documents/Cline/Rules or .clinerules/) if they don't exist.
The Toggle: This is where the workflow improvement shines. Simply click the switch next to any rule file to enable or disable it.
Toggling 'on' appends the rule's content to the system prompt; toggling 'off' removes it. This immediate control allows for dynamic adjustments that weren't practical before.
Shifting Cline's Focus: Like Changing Gears On Demand
Think of your .clinerules files (both global and workspace) as defining specific instruction sets or operational configurations for Cline. Each rule file can encapsulate a particular focus, persona, or set of standards. The toggle UI then becomes your control panel for instantly switching Cline between these configurations as your own focus shifts during development.
Here's how you can leverage this:
Define Task-Specific Configurations: Create granular rule files for common development activities. Examples:
debug-logging.md: Instructs Cline to add detailed logging during debugging.
test-generation-jest.md: Guides Cline on writing Jest unit tests according to your patterns.
refactor-dry-principles.md: Focuses Cline on identifying and reducing code duplication.
docs-technical-style.md: Enforces your team's technical documentation style.
commit-conventional-format.md: Ensures commit messages follow a specific standard.
Switch Contexts Fluidly: Instead of starting new chats or manually editing instructions, simply toggle the relevant rule(s) on or off.
Example: You're fixing a bug, so you activate debug-logging.md. Once fixed, you toggle it off and activate test-generation-jest.md to write a regression test. Then, toggle that off and activate commit-conventional-format.md before committing. Cline seamlessly adapts its behavior at each stage, guided by the active instruction set, all within the same conversation.
Using Memory Bank for some projects, but not all? Add memory-bank.md to your Global Rules and toggle it on when you need it.
Combine Instruction Sets: Need Cline to follow both React best practices and your project's specific component library guidelines? Toggle both react-best-practices.md (global) and project-component-library.md (workspace) on simultaneously. The rules are combined in the system prompt.
Leverage Mid-Task Pivots: As mentioned earlier, the ability to toggle mid-task while preserving conversation history is key. If you're deep in implementing a feature (feature-x-logic.md active) and realize a refactoring opportunity, you can instantly switch Cline's focus by toggling on refactor-dry-principles.md without losing the context of the feature work. Address the refactor, then toggle back to your feature rule. 
Note: switching rules mid-task can be incredibly powerful as you leverage the same context but with a new instruction set. However, it does come at a cost, as modifying the .clinerules does break the prompt cache.
By thinking of your .clinerules as distinct, switchable configurations, you can guide Cline much more precisely and efficiently, adapting its core instructions to match the specific demands of each development phase or task.
Self-improving Cline: Cline Can Write and Refine Its Own Rules
Here's where .clinerules truly diverge from the static "Custom Instructions" field in your settings. Because rules are just .md files in your workspace or global rules folder, Cline itself can create and modify them using its file editing tools.
This unlocks a powerful meta-capability:
Automate Workflow Definition: Have a repetitive task or a specific output format you want Cline to follow consistently? Instead of manually writing the rule, ask Cline to create a new .clinerules file defining that workflow. For example: "Cline, create a new workspace rule named commit-message-format.md that instructs you to always format commit messages following the Conventional Commits standard."
Refine Existing Rules Interactively: If you find a rule isn't working quite right, you don't have to open the file yourself. You can give Cline feedback and ask it to edit the rule directly.
I've found myself asking Cline to improve .clinerules based on feedback throughout a task so much that I've created a "self-improving-cline.md" rule which instructs Cline to autonomously offer suggestions for improving .clinerules. I've added it as a Global Rule:# Self-Improving Cline Reflection

**Objective:** Offer opportunities to continuously improve `.clinerules` based on user interactions and feedback.

**Trigger:** Before using the `attempt_completion` tool for any task that involved user feedback provided at any point during the conversation, or involved multiple non-trivial steps (e.g., multiple file edits, complex logic generation).

**Process:**

1.  **Offer Reflection:** Ask the user: "Before I complete the task, would you like me to reflect on our interaction and suggest potential improvements to the active `.clinerules`?"
2.  **Await User Confirmation:** Proceed to `attempt_completion` immediately if the user declines or doesn't respond affirmatively.
3.  **If User Confirms:**
    a.  **Review Interaction:** Synthesize all feedback provided by the user throughout the entire conversation history for the task. Analyze how this feedback relates to the active `.clinerules` and identify areas where modified instructions could have improved the outcome or better aligned with user preferences.
    b.  **Identify Active Rules:** List the specific global and workspace `.clinerules` files active during the task.
    c.  **Formulate & Propose Improvements:** Generate specific, actionable suggestions for improving the *content* of the relevant active rule files. Prioritize suggestions directly addressing user feedback. Use `replace_in_file` diff blocks when practical, otherwise describe changes clearly.
    d.  **Await User Action on Suggestions:** Ask the user if they agree with the proposed improvements and if they'd like me to apply them *now* using the appropriate tool (`replace_in_file` or `write_to_file`). Apply changes if approved, then proceed to `attempt_completion`.

**Constraint:** Do not offer reflection if:
*   No `.clinerules` were active.
*   The task was very simple and involved no feedback.



This ability for Cline to modify its own guiding instructions turns rule management into a dynamic, collaborative process, allowing you to build a highly personalized and self-improving AI assistant.
Getting Started & Sharing Your Rules
Update Cline: Make sure you have v3.13 or later.
Organize Your Rules: Think modularly. Break down broad instructions into focused .md files (e.g., error-handling.md, typescript-style.md, database-schema-rules.md). Use the '+' button in the popover to create them in the right scope (Global or Workspace). Remember, Cline creates the folders automatically.
Experiment: Play with toggling rules. See how activating different combinations affects Cline's responses. Try the mid-task toggle when you need to pivot while keeping context.
Learn More: For deeper dives, check the prompting docs: https://docs.cline.bot/prompting/README.md
Share with the community! What clever rules are you creating? How are you combining them? Share your .clinerules files and strategies with the community! Post them on Reddit (https://www.reddit.com/r/cline/) or discuss ideas on Discord (https://discord.gg/cline). Let's build a shared library of effective instructions.---


This blog was written by Nick Baumann, Product Marketing at Cline. Follow us @cline for more insights into the future of development.
Install Cline
Join our community: Discord & Reddit