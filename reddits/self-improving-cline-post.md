**Title:** My Workflow for a "Self-Improving Cline"

Hey everyone, Nick here.

I wanted to share a workflow I've found really powerful for making Cline "self-improving."

The core idea came about because I realized I was constantly asking Cline things like, "Based on our conversation, how would you improve the X rule we're using?" It struck me that Cline could automate this reflection process itself -- essentially, teach Cline how to prompt itself to get better.

**How it Works:**

Since `.clinerules` are just markdown files, Cline can edit them using its standard file tools. As you work through a task and provide guidance or corrections (even implicitly through conversation), you can ask Cline to update the *specific, active* `.clinerules` file to incorporate that feedback.

This creates a dynamic loop:
1.  You work with Cline, guided by active `.clinerules`.
2.  Your conversation provides natural feedback on how well the rules are working.
3.  You ask Cline to modify the relevant rule file based on that feedback.
4.  The rule is improved, leading to better alignment in future tasks using that rule.

**The Benefit:**

This turns personalization into an ongoing, collaborative process. Cline becomes progressively more aligned with your specific needs, coding style, and project standards because it's learning *from* your guidance.

**Example:**

Imagine you have a `commit-format.md` rule. If Cline generates a commit message that's missing the scope, you can say: "Cline, let's ensure the scope is always included. Update `commit-format.md` to reflect that." Cline updates the rule, and future commits using it will be better formatted.

**Automating the Reflection: The `self-improving-cline.md` Rule:**

So, to streamline this, I created a rule that basically asks Cline to do what I was doing manually -- reflect on our interaction and suggest improvements to the active rules *before* finishing a task.

If you want to try this workflow yourself, add the following rule (`self-improving-cline.md`) to your Global (`~/Documents/Cline/Rules`) or Workspace (`.clinerules/`) rules:

```markdown
# Self-Improving Cline Reflection

**Objective:** Offer opportunities to continuously improve `.clinerules` based on user interactions and feedback.

**Trigger:** Before using `attempt_completion` for tasks involving feedback or multiple steps.

**Process:**
1. Offer Reflection: Ask user about reflecting on `.clinerules`.
2. Await Confirmation: Proceed if declined.
3. If Confirmed:
    a. Review Interaction & Feedback.
    b. Identify Active Rules.
    c. Propose Rule Improvements.
    d. Await Action & Apply if approved.

**Constraint:** Don't offer if no rules active or task was simple.
```

With this rule active, Cline will ask if you want it to reflect on your interaction and suggest changes to the rules used during the task *before* completing it.

**Get Started:**

Try incorporating this workflow. Guide Cline to refine its rules based on your feedback, and consider adding the reflection rule for proactive suggestions.

Let me know what you think or if you have other cool `.clinerules` workflows!

Relevant Blog Post: [Link to blogs/mastering-context-with-toggleable-clinerules.md when published]
Docs: `https://docs.cline.bot/prompting/custom-instructions.md`
