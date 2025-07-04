# Everyone's Talking About R1 vs o1 Benchmarks. But Here's What Really Matters.

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

January 23, 2025 • 2 min read

In an interesting coincidence, DeepSeek released R1 on the same day we launched Plan & Act modes in Cline. And something fascinating started happening immediately: developers began naturally using R1 for planning phases and 3.5-Sonnet for implementation. Not because anyone suggested it – it just made sense.

0:00
/0:54

1×

## What's Actually Happening

Here's what developers discovered works best:

1. Start new tasks in Plan mode using R1 ($0.55/M tokens)
2. Have a proper planning conversation - discuss architecture, edge cases, potential approaches
3. When ready to build, switch to 3.5-Sonnet
4. If you need to revisit planning or hit complexity, switch back to R1

![](https://cline.ghost.io/content/images/2025/01/image-18.png)
## The Numbers That Matter

Let's talk about why this pattern emerged:

* Planning with R1: $0.55/M tokens
* Planning with 3.5-Sonnet: ~$16/M tokens
* 97% cost reduction for planning phases

But this isn't just about cost savings. As Austin Starks noted in his [recent analysis](https://medium.com/%40austin-starks/the-chinese-obliterated-openai-a-side-by-side-comparison-of-deepseek-r1-vs-openai-o1-for-finance-93a1b4343a82?ref=cline.ghost.io), R1 matches or surpasses other models in reasoning benchmarks. When you combine this with Sonnet's proven implementation capabilities, you get the best of both worlds.

## Why This Pattern Works

The magic happens because you're using each model's natural strengths:

### Planning Phase (R1)

* Deep architectural thinking
* Edge case exploration
* System design decisions
* Cost-effective reasoning

![](https://cline.ghost.io/content/images/2025/01/image-22.png)
### Implementation Phase (3.5-Sonnet)

* Precise code generation
* Complex refactoring
* Bug fixes
* Battle-tested reliability

![](https://cline.ghost.io/content/images/2025/01/image-20.png)
## How to Use This Workflow

Want to try this approach? Here's the process:

1. Start your task in Plan mode with R1
2. Have a proper planning conversation
3. When ready to write code, switch to Sonnet
4. Need to revise the plan? Switch back to R1

0:00
/0:10

1×

## The Bigger Picture

This isn't about R1 vs. o1 or 3.5-Sonnet – it's about using the right tool at the right time. The future of AI development isn't about finding one perfect model, it's about knowing when to use each model's strengths.

And sometimes the best patterns emerge naturally from the community rather than being designed. That's exactly what happened here – developers organically discovered this workflow on release day, and the results speak for themselves.

Let me know in our [Discord](https://discord.gg/cline?ref=cline.ghost.io) or [r/cline](https://www.reddit.com/r/CLine/?ref=cline.ghost.io): Have you tried this R1/Sonnet workflow? What other model combinations have you found effective?

Remember: The goal isn't to pick sides in the model wars. It's to build better software by using the right tool at the right phase of development.
