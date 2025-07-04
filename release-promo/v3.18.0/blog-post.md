---
title: "Cline v3.18: Gemini CLI Provider, Optimized Claude 4"
date: 2025-06-26
author: Nick Baumann
---

Hello Cline community 🫡

Cline v3.18 is a focused release that introduces a powerful new way to use Gemini models, delivers significant performance and reliability upgrades for the Claude 4 family, and ships several important core improvements.

### Gemini CLI Provider

We're always looking for ways to give you more flexibility in how you use Cline. With this release, we've added a new Gemini CLI provider. If you have the Gemini CLI tool installed and authenticated with your personal Google account, you can now leverage it directly within Cline. This gives you access to 1,000 free requests per day for the Gemini 2.5 Pro and Flash models, making it an excellent, cost-effective option for your development workflow. A special thanks to the team at Google for making this possible.

### Major Optimizations for Claude 4

We've invested significant effort in optimizing Cline's integration with the Claude 4 family of models. These aren't just minor tweaks -- they are fundamental improvements that result in better performance, higher reliability, and a smoother user experience. We now recommend the Claude 4 models, particularly Sonnet, as the default for the best results in Cline.

The most critical improvement is in the reliability of our diff-based file editing. In production, we've observed the failure rate for complex diff edits drop from 10% down to just 6%.

[VISUAL: Chart showing diff edit failure rate dropping from 10% to 6%]

These gains are even more pronounced in our internal "hard mode" benchmarks, which test Cline against particularly challenging code modification tasks. On these tests, the success rate for diff edits jumped from 64.4% to an impressive 84.3%.

[VISUAL: Chart showing hard mode benchmark success rate improving from 64.4% to 84.3%]

These optimizations mean fewer interruptions and a more reliable coding partner, allowing you to trust Cline with more complex tasks.

### Other Improvements

This release also includes a few other notable fixes:

*   We've resolved a race condition that could occur when switching between Plan and Act modes.
*   The robustness of our search and replace parsing has been improved to handle more edge cases.
*   The default and recommended model has been officially updated to Claude 4 Sonnet.

### Get Started Today

Cline v3.18 is available now. Update via the VS Code or Cursor marketplace and let us know what you think.

\-Nick 🫡
