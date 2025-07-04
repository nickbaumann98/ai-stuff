# DeepSeek-V3 isn't "free" Claude 3.5-Sonnet. But it's still insanely good for the price.

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

January 5, 2025 • 3 min read

DeepSeek released [V3](https://github.com/deepseek-ai/DeepSeek-V3/tree/main?ref=cline.ghost.io) on December 26, and for the first time since 3.5-Sonnet's release, we have a serious contender for best coding LLM—one that's 53x cheaper and was trained for just $5.5M. Since then, Cline has seen installations skyrocket – nearly 50,000 new installs at double our usual daily rate.

> DeepSeek v3 is mind-blowing. I’m fascinated by the engineering elegance and scrappiness behind it.
>
> - MoE + MLA architecture (671B → 37B active)
> - DualPipe + FP8 , incredibly impressive optimizations
> - $5.5M total cost, just 2 months of training
>
> And the best part? It’s cheaper… [pic.twitter.com/r1G7RHFvmn](https://t.co/r1G7RHFvmn?ref=cline.ghost.io)
>
> — Dina Yerlan (@dina\_yrl) [December 26, 2024](https://twitter.com/dina_yrl/status/1872390117626982687?ref_src=twsrc%5Etfw&ref=cline.ghost.io)

Ten days in, is DeepSeek-V3 reshaping the economics of AI coding? The benchmarks suggest it is, but user feedback is more nuanced. Here’s what Cline users are saying on Discord as they put it to work:

**The Good: It's Shockingly Capable**

"Claude is still king, but I'm shocked at what deepseek can do for less than a penny," notes Saoudrizwan. For many everyday coding tasks, DeepSeek-V3 delivers impressive results at a 2% of the cost.

User Weyert relies on DeepSeek-V3 for unit tests, noting, "DeepSeek is surprisingly good at fixing my broken tests."

As kaustav.gh puts it, "When it works it gives great elaborate solutions almost as good as 3.5 sonnet."

0:00
/0:38

1×

DeepSeek-V3 creating a landing page (2x speed)

0:00
/0:53

1×

Claude 3.5-Sonnet creating a landing page (2x speed)

For frontend tasks, Claude 3.5-Sonnet stands out with its ability to leverage Computer Use (as demonstrated above) and interpret images effectively, both tools that DeepSeek-V3 does not have.

**Reality Check: The Complexity Ceiling**

As projects grow more complex, the limitations become clear. "It keeps saying the task is completed successfully when it's not... deepseek v3 seems drunk," reports thetoni1597, who eventually switched back to Claude at $2-5 per session.

![](https://cline.ghost.io/content/images/2025/01/image-1.png)

DeepSeek-V3 maintains parity with Claude 3.5 Sonnet until reaching a complexity threshold, after which success rates drop significantly

The problems compound quickly. Maxcritreviews didn't mince words: "It isn't even close - it is completely failing at almost everything and not remembering anything." Kaustav.gh noticed that "when the chat gets long it starts hallucinating, unlike sonnet."

The context window keeps coming up - "I wished deepseek had higher context length keep hitting the limitation with cline," notes weyert, a limitation that becomes particularly acute in larger projects (DeepSeek-V3 has a context window of 64k tokens compared to 3.5 Sonnet's 200k context window).

DeepSeek-V3 excels at targeted tasks like unit test fixes but struggles with larger, more complex projects - especially when context and precision matter.

**The Bottom Line**

DeepSeek V3 delivers 3.5-Sonnet-level results for simple tasks at just 2% of the cost. Developers are leveraging this advantage: using DeepSeek V3 for fast development and Sonnet for complex, precision-driven work.

![](https://cline.ghost.io/content/images/2025/01/image-4.png)

DeepSeek-V3 is an exceptional value for lower-complexity tasks

"I haven’t had great results with DeepSeek-V3," admits soyhenry, "but I’m not using [a context management system]." This user has since updated their stance (1/22/25), noting that it is better at handling "very targeted tasks, and in my case, related to unit testing. Or, when Sonnet goes into circles, I bring in DeepSeek to get a different perspective, as it approaches it differently."

Senor1854 suggests, "Cline’s prompts could be optimized for DeepSeek," while ciberninja adds, "It needs extra prompting for tasks like appending to a file." These insights highlight a key truth: DeepSeek-V3 excels with the right approach.

For many developers, it’s an opportunity—use DeepSeek-V3 for rapid prototyping and simpler tasks with proper prompting and context management, then switch to 3.5-Sonnet for precision and complexity. As one user summed it up: "I like it; it’ll make Claude and OpenAI rethink pricing."

**What This Means for Builders**

DeepSeek-V3 isn’t "basically free" 3.5-Sonnet, but it’s by far the best value model available for Cline. It also highlights the direction this market is heading. As inference costs continue to drop and open models improve, the gap between performance and price will keep shrinking. DeepSeek-V3 offers a glimpse of the future: high-end AI capabilities at a fraction of today's costs, making tools like Cline nearly free to use. We're not there yet, but the economics of AI development are shifting fast.

---

Want in on the conversation? Join the Cline Discord [here](https://discord.gg/Adc8sCj3?ref=cline.ghost.io)
