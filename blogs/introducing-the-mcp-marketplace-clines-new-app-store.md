# Introducing the MCP Marketplace: Cline's New App Store

![Nik Pash](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F02%2Fprof-pic-upscaled--1-.png&w=96&q=75)

Nik Pash

February 19, 2025 • 2 min read

Remember when installing new apps meant typing cryptic commands into a terminal, manually resolving dependencies, and praying nothing would break? That's kind of where we are with Model Context Protocol (MCP) servers right now. But not anymore. Today, I'm excited to announce Cline's MCP Marketplace - think of it as the App Store for your AI's capabilities. It's our answer to making AI superpowers accessible to everyone, not just the tech-savvy few.

## Why This Matters

A few months ago, Anthropic released the Model Context Protocol - a fancy way of saying "hey, let's standardize how AIs talk to external tools." Cool concept, but like many great technologies, the initial setup process was about as fun as filing taxes. We saw this firsthand at Cline. Users loved the power of MCPs but hated the setup process. They'd have to:

* Find the right GitHub repo
* Read through technical documentation
* Configure JSON files manually
* Cross their fingers and hope it works

Not exactly the "future of AI" experience we were aiming for.

## Enter the MCP Marketplace

Here's what we built: a clean, simple interface where you can:

* Browse available MCP servers
* See ratings, downloads, and descriptions
* Install any MCP with a single click
* Get automatic setup and configuration

No more JSON wrangling. No more dependency hell. Just click and let Cline handle the rest.

## How It Works

1. Open Cline in VS Code (we just hit 700,000 downloads, by the way - thanks everyone!)
2. Navigate to the MCP Marketplace
3. Find an MCP server you want (we've got everything from Figma integration to web search)
4. Click "Download"
5. Let Cline handle the setup

That's it. Cline reads the installation instructions, asks you for any necessary API keys, and configures everything automatically.

0:00
/0:30

1×

## For MCP Developers

If you're building MCP servers (you wonderful human, you), we're introducing a new standard: the `llms-installation.md` file. It's a dedicated set of instructions that helps AI agents like Cline install your MCP server reliably. Think of it as writing instructions for a very capable but literal-minded junior developer. Include:

* Required dependencies
* API key requirements (both required and optional)
* Step-by-step installation process
* Common troubleshooting tips

Want to get your MCP server listed? Create an issue in our [mcp-marketplace repo](https://github.com/cline/mcp-marketplace?ref=cline.ghost.io) with:

1. Your GitHub repo URL
2. A 400x400 PNG logo
3. A brief description of why it should be included

## What's Next

This is just the beginning. As our marketplace grows, we're seeing incredible MCPs being built - from code analysis tools to design integrations. The possibilities are endless, and we can't wait to see what you build. If you're already using Cline (thank you!), the MCP Marketplace update is rolling out now. If you haven't tried Cline yet, well, there's never been a better time to give your AI some superpowers. Want to stay updated on Cline and get early access to new features? Subscribe to our newsletter below. We're building the future of AI development, and we'd love to have you along for the ride. —

*PS: If you're building something cool with MCPs, I'd love to hear about it. Reach out on Twitter!*
