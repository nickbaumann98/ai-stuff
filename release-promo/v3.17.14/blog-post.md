---
title: 'Cline v3.17.14: New Provider Options, Terminal Upgrades, and Core Fixes'
date: '2025-06-18'
author:
  name: Nick Baumann
  image: 'https://cline.ghost.io/content/images/2025/01/ProfilePicture.jpg'
---

Hello Cline community 🫡

v3.17.14 is a patch focused on expanding provider support, refining the terminal experience, and shipping a handful of important stability improvements.

### New Provider Integrations

We're committed to making Cline as flexible as possible, and that means letting you plug in the tools you already use. This release adds support for two new API providers.

*   **Claude Code:** If you have Anthropic's Claude Code CLI tool installed locally, you can now use it as a provider within Cline. This allows you to leverage your Claude Max Plan directly in Cline.
*   **SAP AI Core:** We've also added support for SAP AI Core, enabling users to connect to both Claude and GPT models through the service. A big thank you to @schardosin for contributing this integration.

### Terminal Experience Upgrades

We've made two quality-of-life improvements to how Cline interacts with your terminal.

First, you can now set a default terminal profile in Cline's settings. This gives you control over which terminal Cline uses for its commands, which should help work around some persistent shell integration bugs. Thanks to @valinha for this addition.

Second, a new setting allows you to constrain the terminal output size. This prevents Cline from being overwhelmed by commands that produce an excessive amount of text, making for a smoother experience.

### Core Improvements and Fixes

This release also includes several under-the-hood fixes to improve reliability.

*   **Checkpoint and Task Reliability:** We've resolved issues with task restoration and checkpoint saving to ensure file changes are tracked more accurately, reducing errors when resuming work.
*   **Search and Replace:** The search and replace algorithm is now more lenient, fixing an edge case that could cause file deletion with certain diff formats.
*   **AWS Bedrock:** The Bedrock provider has been updated to use the standard AWS SDK, removing a deprecated dependency. Thanks, @watany-dev.
*   **And More:** We've also fixed the `list_files` tool for hidden directories, improved the MCP Rich Display settings (thanks @Vl4diC0de!), and refactored our copy button components (thanks @shouhanzen!).

### Get Started Today

Cline 3.17.14 is available now. Update and let us know what you think!

-Nick 🫡
