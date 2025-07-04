# Cline v3.15: Unveiling Task Timeline, Gemini Implicit Caching & New Community Docs

Welcome to Cline v3.15! We're excited to share a release that’s all about refining your AI coding experience, bringing you clearer insights, smarter efficiencies, and deeper community collaboration. This isn't just an update; it's a reflection of our ongoing conversation with you, our users, and our commitment to making Cline an indispensable partner in your development journey. We've focused on enhancements that you'll feel every day, making complex tasks more transparent and your workflow smoother.

Let's explore what's new.

## Task Timeline: A Clearer View of Cline's Journey

Ever wished you could instantly see the "story" of how Cline tackled a complex task? With v3.15, we're introducing the **Task Timeline**, a sleek, visual "storyboard" integrated directly into your task header. This isn't just a log; it's an intuitive series of blocks charting every key step Cline takes – from tool calls to file edits. Hover over any block, and you get an instant summary of the action and its timestamp. `[VISUAL: Task Timeline Screenshot - showing hover preview]`

The beauty of the Task Timeline lies in its ability to provide deep transparency effortlessly. You can now understand complex agent actions at a glance, easily review past work for insights, and even spot patterns to refine your collaboration with Cline. This feature, a nod to our vision for future multi-agent visibility and built with the talent of community contributor `eomcaleb`, makes understanding Cline more intuitive than ever. It’s about transforming abstract processes into a clear, visual narrative. `[VIDEO: Task Timeline Demo]`

> **Pro Tip: Quick Task Review & Learning**
> Before diving deep into a long task's transcript, use the Task Timeline to quickly grasp the main stages and tool interactions. It’s also invaluable for learning: if a task veered off course, the timeline can help pinpoint exactly where, offering insights for future prompting.

## Gemini Implicit Caching: Affordable Power

Leveraging the cutting edge of AI like Google's Gemini 2.5 Pro should be empowering, not prohibitively expensive. We heard your feedback on the previous costs and complexities, and we're thrilled that, following community input and our team's advocacy (kudos to Nik Pash (pashmerepat) for championing this), the Google Gemini team (including Logan Kilpatrick (@OfficialLoganK)) has rolled out **Implicit Caching**. Cline v3.15 seamlessly integrates this, translating to significant, automatic savings for you. `[VISUAL: Screenshot of Logan Kilpatrick's tweet]`

Now, when you're working iteratively with Gemini 2.5 Pro, repetitive portions of your prompts can benefit from up to a 75% token discount, with no manual setup required. This makes one of the most powerful models on the market considerably more accessible and affordable. `[VISUAL: Cache UI indication for Gemini if applicable, or conceptual graphic]` It’s a prime example of how community feedback and collaborative engagement with model providers can lead to tangible benefits for every developer using Cline.

## Community-Powered Documentation: Building Cline's Knowledge Together

Great software thrives on great documentation, and we believe the best documentation is built *with* the community it serves. That's why we've undertaken a significant overhaul: Cline's documentation has migrated to the excellent Mintlify platform and, more importantly, now lives directly within our main open-source repository on GitHub. `[VISUAL: Screenshot of new Mintlify docs interface]`

This move is all about accessibility and collaboration. Found a typo, have a clearer explanation for a feature, or want to share a useful workflow? Now, contributing to the docs is as straightforward as submitting a pull request for code. It ensures our documentation remains a living, breathing resource – accurate, up-to-date, and enriched by the collective wisdom and experience of Cline users like you. `[VISUAL: Example of an easy documentation contribution on GitHub]`

> **Your First Cline Contribution is Easier Than You Think!**
> Looking to contribute to Cline? Improving the docs is a fantastic entry point. Start by clarifying a sentence, adding a missing link, or expanding on an example for a feature you use regularly. Every contribution, no matter how small, enhances this shared resource.

## Non-Blocking UI: Stay in Your Flow, Uninterrupted

One of the most impactful changes to your daily workflow in v3.15 comes directly from the kind of invaluable, hands-on feedback we cherish. Designer and MCP contributor Siddharth Ahuja (sidahuj), known for his innovative work on tools like the Blender and Ableton MCP servers, recently visited the Cline office. We had the opportunity to sit down with him for a couple of hours, simply observing him use Cline and listening to his insights. What stood out most was his experience during file edits: while appreciating the transparency, he highlighted the frustration of being locked out, unable to interact further while Cline worked.

His direct feedback was the catalyst for the new **Non-Blocking UI**. No more waiting. Now, as Cline diligently works on writing to files or applying diffs, your interface remains fully responsive. You can type your next message, scroll through the active file, or navigate the UI without interruption. `[VIDEO: Demo of Non-Blocking UI - showing typing/scrolling while Cline edits]` This seemingly small change, born from direct user observation, has a big impact, making your interaction with Cline feel significantly smoother, more fluid, and respectful of your focus. You stay in control, and you stay in the creative flow.

> **Pro Tip: Leverage the Lag-Free Edits**
> Use those moments while Cline is editing to your advantage. Review another section of code, prepare your next prompt, or update your context files. This ability to multitask seamlessly can noticeably speed up your development cycles.

## Key Quality-of-Life Updates & Community Contributions

Beyond these headline features, Cline v3.15 is brimming with refinements and additions that polish your experience:

*   **Quote Previous Message:** For more precise communication, you can now easily quote parts of earlier messages in the chat. This is perfect for providing targeted feedback, asking for clarification on a specific point, or refining plans with pinpoint accuracy. `[VISUAL: Screenshot of Quoting Message in Chat]` / `[VIDEO: Demo of quote message for better plan feedback]`
*   **Larger File Analysis:** We've enhanced Cline's ability to handle larger individual files, allowing you to better utilize the expansive context windows of models like Gemini 2.5 Pro. `[VISUAL: Conceptual graphic of large file being processed]`
*   **Improved Terminal Stability:** We've squashed critical bugs that could cause terminal commands to hang or lock out tasks, leading to a more reliable experience.
*   **Simplified Home Header:** Enjoy a cleaner, more streamlined look when you first open Cline. `[VISUAL: Screenshot of Simplified Home Header]`
*   **Enhanced Copy Functionality:** More convenient copy buttons are now available for task headers, assistant messages, code blocks, and markdown sections. (Thanks weshoke!) `[VISUAL: Screenshot of new Copy Buttons]`
*   **Favorite Tasks:** Keep important or ongoing tasks readily accessible by marking them as favorites, even when clearing your history. `[VISUAL: Screenshot of Favorite Tasks feature]`
*   **AI-Assisted Commit Messages:** Let Cline help draft your commit messages based on the context of your task. (Thanks zapp88!) `[VISUAL: Demo/Screenshot of Commit Message Generation]`
*   **Better Integration with Cursor & Windsurf:** Cline now offers an improved UI for managing rules in these environments. `[VISUAL: Screenshot of Windsurf/Cursor Rules UI in Cline]`
*   **Redesigned Auto-Approve UI:** Managing auto-approve settings is more intuitive, now featuring a handy "Approve All Commands" button for power users. `[VISUAL: Screenshot of new Auto-Approve UI with 'Approve All' button]`
*   **`/reportbug` Slash Command:** A quick and easy way to report issues with contextual information directly from the Cline chat.
*   **Batch History Deletion:** Efficiently manage your task history by selecting and deleting multiple tasks at once. (Thanks danix800!) `[VISUAL: Demo of Batch History Deletion]`

And that’s not all! This release also includes support for the Mistral Medium-3 model, various updates for Bedrock models (thanks Watany!), and a host of other fixes and smaller improvements thanks to the diligence of our community contributors like PeterDaveHello, DaveFres, WinterYukky, and many others.

Our heartfelt thanks to everyone in the Cline community. Your feedback, contributions, and enthusiasm are what drive us forward. 🙏

## Get Started with v3.15

Cline v3.15 is all about making your interaction with AI smoother, more insightful, and more collaborative. We believe these updates will make a tangible difference in your daily development work.

Dive in, explore the new features, and let us know what you think!

*   **Read the full [Changelog](https://github.com/cline/cline/blob/main/CHANGELOG.md)**
*   **Explore our new [Community Docs](https://docs.cline.bot)** (Note: URL may be updating)
*   **Join the discussion on [Reddit](https://www.reddit.com/r/cline/)**
*   **Chat with us on [Discord](https://discord.gg/cline)**
*   **If Cline is helping you build faster, please consider [leaving a review](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev). It makes a huge difference!**

Happy Coding!
