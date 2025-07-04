# Why AI Engineers Need Planning More Than Perfect Prompts

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

January 21, 2025 • 4 min read

The best AI engineers I know follow a specific pattern. They don't obsess over prompt crafting – they obsess over planning. There's a reason for this, and it's not what most people think.

## The Reality Check

Here's what typically happens when someone starts working with AI:

1. They throw requirements at the model
2. They get mediocre outputs
3. They blame their prompting skills
4. They spend hours "optimizing" prompts
5. They still get mediocre results

Sound familiar? But here's what elite AI engineers do instead: they treat AI like a junior developer who needs context to succeed. They spend time explaining the project, sharing constraints, and outlining goals before writing a single line of code.

## Why Context Matters More Than Prompts

![](https://cline.ghost.io/content/images/2025/01/image-15.png)

Think of AI outputs like bullets from a gun (bear with me on this analogy). The more context you provide, the longer the barrel becomes – and longer barrels mean better accuracy. Our power users have discovered this naturally: when they take time to plan and provide context before coding, Cline's outputs became significantly more precise.

This is why Cline doesn't artificially cap context or optimize for token efficiency. And it's why I get frustrated when I see companies artificially limiting context to save on tokens. It's like shortening your gun barrel to save on metal – you're sacrificing accuracy for economy.

Cline instead reads entire codebases, digests documentation, and maintains deep context throughout your session. Yes, this means higher token usage, but it also means the difference between an AI that suggests code and one that truly understands your project. It's like the difference between shooting at a target with a pistol versus a precision rifle – both can hit the mark, but one is deliberately engineered for accuracy.

## The Two Modes Every AI Engineer Should Use

We've formalized this workflow into two distinct modes which you should be using to build with Cline:

**Plan Mode**

* Optimized for context gathering and strategy
* Will collaborate with you on a plan; will NOT write code
* Full file-reading capabilities for project understanding
* Focused on breaking down complex requirements and producing a plan

![](https://cline.ghost.io/content/images/2025/01/image-16.png)

**Act Mode** (the Cline you know well)

* Streamlined for implementation based on provided context
* Executes against the established plan
* Maintains full access to Cline's building capabilities

![](https://cline.ghost.io/content/images/2025/01/image-17-1.png)
## How It Looks in Practice

**1) Start in Plan Mode**

* Share your requirements
* Cline reads relevant files and asks clarifying questions
* Together, you develop an implementation strategy

Here's a real example:

> "I want to improve the SEO of our landing page. How can we do that"

Cline will then investigate your codebase for relevant files and any documentation or context files which are in your project.

> Cline: "After analyzing the current HTML file, I've identified several opportunities to improve the SEO of the Polaroid landing page. Here's a comprehensive plan to enhance its search engine optimization:
>
> {...rest of plan}
>
> Would you like me to proceed with implementing these improvements? If so, please toggle to**Act mode**and I'll start making these enhancements systematically."

0:00
/0:15

1×

Use Plan mode to create an implementation plan before building

**2) Switch to Act Mode**

* Cline shifts into builder mode
* Executes against the agreed plan
* Maintains context from planning phase

0:00
/0:29

1×

Switch to Act mode after a plan has been made

**3) Iterate as Needed**

* Seamlessly switch between modes
* Planning isn't a one-time thing
* Complex projects often require multiple plan-act cycles

0:00
/0:25

1×

Switch back to Plan mode to course correct Cline

Remember:

**Plan**mode can't make any changes to your codebase. Use Plan mode when you want to talk to Cline.

**Act** mode has access to all tools (it's the regular Cline you're used to). Use Act mode when you want Cline to build.

## Why This Matters

The implications here go beyond just getting better AI outputs. This approach:

1. Saves time in the long run
2. Produces more maintainable code
3. Catches edge cases early
4. Creates better documentation naturally
5. Makes iteration easier

## Power User Tips

* Use Plan mode to explore edge cases before implementation
* Switch back to Plan when encountering unexpected complexity
* Leverage file reading to validate assumptions early
* Have Cline write markdown (.md) files of the plan as context it can reference in the future

## The Hard Truth

Look, I get it. Planning feels slow. It feels like you're not "doing" anything. But here's the truth: the time you spend planning pays for itself many times over in the quality of your outputs.

The best AI engineers I know aren't necessarily the ones who write the most elegant prompts. They're the ones who take the time to think through problems thoroughly before diving into implementation.

## Where to Go From Here

If you're building AI systems, try this: For your next project, spend twice as long as you normally would in the planning phase. Document everything. Share all the context you can. Then start building.

I bet you'll be surprised by the difference in output quality.

If you're building something interesting with Plan & Act modes, we want to know about it. Share your experiences in our Discord or drop your thoughts in this Reddit thread. Your feedback directly shapes how we evolve these features.
