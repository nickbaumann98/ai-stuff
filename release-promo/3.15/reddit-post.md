**Title:** Cline v3.15 Released: Task Timeline, Gemini Implicit Caching, Community Docs, Quote Replies & More!

**Body:**

Hey everyone,

Excited to share Cline v3.15 is out! 

Here are the highlights:

**Task Timeline: Visualize Your Cline's Workflow**
Get a better view of your conversation with Cline a "storyboard" of key actions right in the task header. You'll see tool calls, file edits, and other significant events as a sequence of blocks – just hover for a quick summary. It’s perfect for easily grasping complex agent actions, reviewing past tasks, and spotting patterns. `[VISUAL: Task Timeline Screenshot - showing hover preview]` `[VIDEO: Task Timeline Demo]`

**Gemini Implicit Caching: Powerful AI, Smarter Spending**
Using Gemini 2.5 Pro just got significantly more cost-effective! Cline v3.15 seamlessly integrates Google's new [Implicit Caching](https://developers.googleblog.com/en/gemini-2-5-models-now-support-implicit-caching/). This means you can benefit from up to 75% token discounts on repetitive prompt portions automatically, without any manual setup. It's a big step in making powerful AI more accessible, addressing community feedback on previous Gemini costs. We appreciate the Google Gemini team's responsiveness in rolling out this improvement! `[VISUAL: Screenshot of Logan Kilpatrick's tweet]` `[VISUAL: Cache UI indication for Gemini if applicable, or conceptual graphic]`
*Pro Tip: For Gemini 2.5 Pro, keep core instructions at the start of your prompt and new queries at the end to maximize cache hits.*

**Community-Powered Documentation: Build with Us!**
Our [docs](docs.cline.bot) have moved to Mintlify and are now in the main Cline [open-source repo!](https://github.com/cline/cline/tree/main/docs) This makes it much easier for you, our community, to contribute to and improve Cline's documentation. Help us keep them accurate, comprehensive, and reflective of best practices by submitting PRs for doc improvements just like you do for code. `[VISUAL: Example of an easy documentation contribution on GitHub]` `[VISUAL: Screenshot of new Mintlify docs interface]`
*Pro Tip: A great first doc contribution can be as simple as clarifying a sentence or adding an example!*

**Non-Blocking UI: Stay in Your Flow**
No more waiting while Cline edits files! Inspired by valuable user feedback, our UI now stays fully responsive during these operations. You can type your next message, scroll files, or navigate the UI while Cline applies changes, leading to a much smoother and more fluid workflow. `[VIDEO: Demo of Non-Blocking UI - showing typing/scrolling while Cline edits]`

**New `/reportbug` Slash Command**
We've made it easier to help us improve Cline! The new `/reportbug` slash command lets you report issues directly from the chat, automatically including contextual information. Your detailed bug reports are invaluable. `[VISUAL: Screenshot of /reportbug command in action]`

**Key Quality-of-Life Updates & Community Contributions**
This release is also packed with other significant improvements:
*   **Quote Previous Message:** For more precise communication and feedback. `[VISUAL: Screenshot of Quoting Message in Chat]`
*   **Larger File Analysis:** Cline now better handles larger individual files with high-context models. `[VISUAL: Conceptual graphic of large file being processed]`
*   **Improved Terminal Stability:** Significant fixes to reduce terminal-related task lockouts.
*   **Simplified Home Header:** A cleaner, more streamlined look. `[VISUAL: Screenshot of Simplified Home Header]`
*   **Enhanced Copy Buttons:** More convenient copying from task headers, messages, and code blocks. (Thanks weshoke!) `[VISUAL: Screenshot of new Copy Buttons]`
*   **Favorite Tasks:** Mark tasks as favorites to keep them when clearing history. (Thanks zapp88 for the commit message feature also!)
*   **UI for Windsurf & Cursor Rules:** Improved integration for users of these environments. `[VISUAL: Screenshot of Windsurf/Cursor Rules UI in Cline]`
*   **Updated Auto-Approve UI:** More intuitive, with an "Approve All Commands" button. `[VISUAL: Screenshot of new Auto-Approve UI with 'Approve All' button]`
*   **Batch History Deletion:** Select and delete multiple tasks at once. (Thanks danix800!) `[VISUAL: Demo of Batch History Deletion]`
*   **Plus:** Support for Mistral Medium-3, Bedrock model updates (thanks Watany!), and many other fixes (thanks PeterDaveHello, DaveFres, WinterYukky!).

Huge thanks to all community contributors! 🙏

Read the full details in our **[latest blog post](LINK_TO_BLOG_POST_HERE)** 📣 Check out the full **[changelog](https://github.com/cline/cline/blob/main/CHANGELOG.md)** for all the details.

Let us know what you think here or on **[Discord](https://discord.gg/cline)**!

Happy coding!

-Nick
