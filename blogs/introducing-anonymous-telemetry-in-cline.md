# Introducing Anonymous Telemetry in Cline

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

February 26, 2025 • 1 min read

At Cline, we're committed to creating the best possible open-source coding agent for developers. Today, we're introducing anonymous telemetry to help us understand how our Cline is actually being used and where we can make meaningful improvements.

**Privacy-First Telemetry**

We've designed our telemetry system with your privacy as the top priority:

* **Completely anonymous** - we use PostHog to collect aggregated usage data that cannot be traced back to individuals
* **Strictly limited scope** - we only collect basic interaction patterns and error events
* **No sensitive data** - we never collect your code, prompts, conversation content, or personal information

**Always Opt-In, Always Your Choice**

Telemetry in Cline is entirely optional and requires your explicit consent:

* When you update or install our VS Code extension, you'll see a simple prompt: "Help Improve Cline" with Allow or Deny options
* You can change your preference anytime in settings

**Why This Helps Us Make Cline Better**

Unlike traditional software, AI tools like Cline present unique measurement challenges. Anonymous telemetry helps us:

* Identify and fix bugs faster
* Understand which features provide the most value
* Make data-driven improvements based on real usage patterns
* Optimize performance across different environments

**Our Ongoing Commitment**

As Cline evolves, our telemetry capabilities may expand to help us solve new challenges. However, our commitment remains unchanged: all data collection will be minimal, anonymous, transparent, and fully under your control.

By enabling telemetry, you're directly helping us build a better Cline for everyone in our community. Thank you for your trust and support.

— The Cline Team

---

*Curious how we implemented telemetry? Cline is open-source, so you can check out the code for yourself* [*here*](https://github.com/cline/cline/blob/main/src/services/telemetry/TelemetryService.ts?ref=cline.ghost.io)*.*
