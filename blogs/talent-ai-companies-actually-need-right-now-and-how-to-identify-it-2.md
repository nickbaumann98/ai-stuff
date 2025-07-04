# What AI Companies Actually Need Right Now

![Nik Pash](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F02%2Fprof-pic-upscaled--1-.png&w=96&q=75)

Nik Pash

February 7, 2025 • 3 min read

At Cline, we've scaled to 500k+ users and raised significant funding from top-tier VCs. As Head of AI, I recently interviewed a strong ML engineer candidate. Despite their solid background, I voted "no hire." Let me explain why - it reveals a broader pattern about what AI companies actually need right now, and getting this wrong can be a $200k+ mistake.

## The $200k Mistake: Why Hiring MLEs Too Early Kills AI Startups

Here's a pattern I see repeatedly in well-funded AI startups:

1. Raise a substantial round with an AI-heavy pitch
2. Rush to hire expensive ML talent to "validate" the AI focus
3. Watch that talent spend months on basic infrastructure
4. Lose them to companies with actual ML challenges

The real cost isn't just the $200k salary - it's the opportunity cost of building the wrong foundations with the wrong team. It's watching your ML experts spend six months debugging TypeScript errors and writing REST APIs instead of doing the work they were hired for.

> **Quick aside: "What's the difference between Machine Learning Engineers and AI Engineers?"**
>
> MLEs and AI Engineers share a lot of DNA - both work with non deterministic systems and both care about building robust systems. The key difference? MLEs typically specialize in training custom models from scratch, like building new engines from raw materials at low levels.
>
> AI Engineers, especially in today's LLM-driven landscape, focus on effectively using and improving existing powerful models - more like mechanics who know how to take a high-performance engine, integrate it into a complete system, measure its performance, and systematically improve how it works in the real world.
>
> Both roles are valuable, but right now most companies need the mechanic before they need the engine builder.

## Patterns in Practice: An Interview Case Study

Let me share a telling interview exchange that illustrates what I mean:

> "Our coding agent sometimes makes suboptimal tool choices - for example, not including jeans when users search for 'pants in denim'. How would you improve this?"

A candidate recently responded:

> "Maybe we could use dropout layers... it feels like it's overfitting too much..."

This kind of response - jumping *straight* to ML architecture before understanding the problem - perfectly illustrates the mindset we need to move beyond.

These aren't wrong answers - they're answers to the wrong problem. They reveal a mindset still anchored in traditional ML when what we need is something quite different.

## What Growing AI Companies Actually Need

At Cline, like many AI companies, our challenges aren't about training models. They're about:

1. Understanding how our systems perform
2. Measuring success systematically
3. Improving behavior methodically

When discussing improvements, I often see this pattern:

> Candidate: "Maybe we could fine-tune the model..."
> Me: "How would we measure if that actually improved things?"
> Candidate: "Oh... we could look at user behavior..."

This guided discovery shouldn't be necessary. The strongest candidates immediately ask:

* *"How do you measure success currently?"*
* *"What signals indicate a tool choice was wrong?"*
* *"What data are you collecting about user interactions?"*

## The New Wave of AI Engineering

What we're seeing is the emergence of a new kind of engineer - one who combines:

1. Systems thinking from traditional software engineering
2. Rigor around non-deterministic systems from ML
3. Practical understanding of LLM capabilities and limitations
4. Focus on measurement and systematic improvement

These engineers are building:

* Sophisticated prompt evaluation frameworks
* Real-time monitoring systems for LLM behavior
* A/B testing infrastructure for prompt improvements
* Clear success metrics that align with business outcomes

At Cline, this has translated into concrete wins:

* Systematic improvement processes that raised success rates
* Clear metrics that drive product decisions
* Scalable systems that grow with our user base

## Red Flags in Interviews

Watch for candidates who:

* Respond with uncertainty rather than curiosity ("I guess maybe...")
* Need to be guided to practical solutions
* Can't independently propose measurement approaches

Here's a pattern I see too often:

> Me: "How would you validate that your changes improved things?"
> Candidate: "I guess we could collect more validation data..."
> Me: "What about user behavior?"
> Candidate: "Oh... right..."

## Green Flags to Look For

The strongest candidates show:

1. Systems thinking about measurement
2. Focus on understanding current behavior
3. Interest in user feedback and metrics
4. Pragmatic approach to improvement

The best responses start with:

> "First, we need to understand what success looks like. Do we have observability into how users use our platform? How do we know when tool selection fails?"

## Building the Right Team

For AI companies building with LLMs, here's what to prioritize:

1. Infrastructure First
   * Robust telemetry
   * Clear success metrics
   * Evaluation frameworks
2. The Right Skills
   * Systems thinking
   * Measurement focus
   * LLM understanding
3. Future Growth
   * Data collection
   * Systematic improvement
   * Scalable architecture

## Looking Ahead

Will we need traditional ML expertise eventually? Absolutely. But first, we need to build the foundations that will make that expertise valuable.

For now, we need engineers who can:

* Build robust measurement systems
* Implement systematic improvements
* Think clearly about LLM behavior
* Create scalable evaluation frameworks

The future of AI engineering isn't just about ML expertise - it's about building systems that can effectively utilize and improve AI capabilities. The sooner we recognize this, the better we'll be at building and scaling AI products.

> If building high-accuracy, trustworthy AI systems at scale excites you, we're looking for engineers who think this way. Please shoot me an email at [nik@cline.bot](https://cline.ghost.io/the-2025-stack-how-complete-beginners-can-ship-their-first-full-stack-web-app/)
