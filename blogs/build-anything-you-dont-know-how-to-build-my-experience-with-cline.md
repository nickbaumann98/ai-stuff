# Build Anything You Don't Know How to Build: My Experience with Cline

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

March 10, 2025 • 3 min read

I've been using Cline since it was released, and it's completely transformed how I approach building software. As Cline's product marketer, I've had the privilege of seeing this tool evolve, but what's more exciting is how it's evolved my own thinking about what I can create.

I produce music on the side, and recently I had this idea: what if I could build a Cline-like assistant for Logic Pro? Something that would let me draw MIDI files and handle mixing through conversation, so I could focus more on what I'm hearing and less on technical details.

There was just one problem – I have no idea how to build Logic Pro extensions. I don't know Swift, I don't know Apple's extension frameworks, and I've never built anything like this before.

But here's the thing: I didn't see that as a limitation. Why? Because months of working with Cline has taught me that not knowing how to build something is no longer a barrier to building it.

## How I'm Building a Logic Pro Extension Without Knowing How

Instead of spending months learning Swift and Logic Pro's development framework, I took a different approach. I used Cline with the Firecrawl Deep Research MCP server to do the heavy lifting for me.

0:00
/0:25

1×

Here's what this looked like in practice:

1. I started by telling Cline exactly what I wanted to build
2. Through the Firecrawl Deep Research MCP server, Cline gathered documentation about Logic Pro extensions
3. Cline analyzed Apple's development guidelines, frameworks, and APIs for audio plugin development
4. All this research was stored within my project repo as documentation
5. Now, Cline could reference this documentation as we worked together on building the extension

The result? I'm actively developing a Logic Pro extension without having to become a Swift expert or Apple extension developer first. I can focus on what the tool should do rather than getting lost in how to implement it.

This approach has been transformative for me since I started using Cline. The traditional development path says "learn first, then build." But with Cline, I've inverted that process – I decide what to build first, then let Cline handle the learning.

It's like having a collaborator who can instantly become an expert in whatever domain we need to work in. This capability has fundamentally changed how I think about what's possible.

## Modifying the Cline Extension Itself

Another example: I wanted to experiment with some optimizations for how Cline builds MCP servers by modifying Cline's extension code. Despite working with Cline daily as a user, I had zero understanding of the extension's internal architecture (I leave that to our brilliant engineers).

In the past, this knowledge gap would have stopped me cold. But now, I no longer see unfamiliarity with a codebase as a barrier – just another knowledge gap that Cline could bridge for me.

0:00
/0:33

1×

So I applied the same principle:

1. Had Cline read through its own extension codebase
2. Asked it to understand the structure and patterns
3. Explained the modifications I wanted to experiment with
4. Cline identified the relevant files and helped me implement the changes
5. It even walked me through testing the VS Code extension to verify everything worked

The pattern is clear: with Cline, the limiting factor isn't my technical knowledge - it's my ability to articulate what I want to build or modify.

## Reframing What's Personally Possible

The most profound insight from all this is how Cline changes what you believe is possible for yourself. When you realize you can build things you don't know how to build, your creativity explodes.

You stop asking "Do I know how to build this?" and start asking "What do I want to build?"

This shift is profoundly empowering. The gap between imagination and implementation virtually disappears. Your only limitation becomes your ability to clearly define what you want to create.

![](https://cline.ghost.io/content/images/2025/03/anythingispossible.gif)
## The Future of Building

We're witnessing a fundamental shift in software development. The technical boundaries and prerequisites that limited who could build what are dissolving.

In this new landscape, your ability to envision and articulate what you want matters far more than your technical background. Cline serves as a universal translator between your ideas and working code.

Whether you're building a Logic Pro extension, managing a website without web development expertise, or modifying a codebase you've never seen before, the principle remains the same: you can build anything you don't know how to build.

Your only limitation might be your imagination – not your technical knowledge or experience.

---

*This blog was written by Nick Baumann, Product Marketing at Cline. Follow us*[*@cline*](https://twitter.com/cline?ref=cline.ghost.io)*for more insights into the future of development.*

[*Install Cline*](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev&ref=cline.ghost.io)

*Join our community:*[*Discord*](https://discord.gg/cline?ref=cline.ghost.io)*&*[*Reddit*](https://reddit.com/r/cline?ref=cline.ghost.io)
