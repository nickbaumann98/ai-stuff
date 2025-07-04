# Draft Reddit Comments – 2025-04-10

---

## Thread: How do you get these AI Assistants to stop guessing and assuming?
https://www.reddit.com/r/ChatGPTCoding/comments/1jw1cjt/how_do_you_get_these_ai_assistants_to_stop/

**Short/Succinct Option:**

You can’t fully stop LLMs from guessing, but you can make a huge difference by managing context tightly. Keep your prompts focused, only include the docs or files you actually need, and start a new session when things get messy. I’ve found that maintaining a short, up-to-date “project context” file and sharing it at the start of each session helps a lot. The more you treat the assistant like a junior dev with a short memory, the better the results.

**Longer/More Detailed Option:**

This is a pain in the a$$ for everyone using AI coding tools right now. The root issue is context management—these models only have so much “working memory,” and when you overload it, they start hallucinating or inventing stuff that isn’t in your docs. The best way I’ve found to keep things on track is to use a dedicated context file: a living doc that summarizes your requirements, key APIs, and any gotchas. Share that at the start of each session, and keep your queries focused on one task at a time. If you’re working on something big, break it into smaller steps and reset the chat when you hit a wall. There’s a good breakdown of this approach here: https://docs.cline.bot/getting-started/understanding-context-management

---

## Thread: What AI coding setup do you use? Cursor, Windsurf, VS Code with CLI tools, Roo Coder, or something else?
https://www.reddit.com/r/ChatGPTCoding/comments/1jvw9ma/what_ai_coding_setup_do_you_use_cursor_windsurf/

**Short/Succinct Option:**

Hey, Nick from Cline here. I obviously have a bias, but I keep coming back to Cline in VS Code. The Plan/Act workflow is a game changer for bigger projects -- you can actually map out your approach, then let the agent handle the code edits step by step. Plus, you can plug in any model (Claude, Gemini, DeepSeek, even local ones) and extend it with MCP servers for custom tools. It’s usage-based, so you only pay for what you use, and you get full transparency on context window usage. If you want something that feels like a real engineering partner, it’s worth a look.

**Longer/More Detailed Option:**

Full disclosure -- I work on Cline. But here's why I love using it (my setup is VS Code + Cline, though I'm curious to try Cursor + Cline too):

*   Model Freedom: I mostly use Gemini 2.5 Pro Exp via OpenRouter which is free and incredibly good. Also keeping an eye on OpenRouter's Quesar Alpha/Optimus stealth models -- also free and look promising. Cline lets you plug in whatever model works best, including local ones.
*   Extensibility with MCP: The Model Context Protocol is huge. I constantly use MCP servers for Perplexity, Firecrawl, and a few custom ones I built myself (Cline is actually great for building these -- just feed it API docs). The MCP Marketplace is making this even easier.
*   Plan/Act Workflow: This feels way more intuitive for complex tasks than just chatting. You plan the steps, review, then let the agent execute. It's like having a real collaborator.
*   Usage-Based = Better Inference: Because it's pay-per-token, Cline doesn't seem to cut corners on inference quality or context handling like some subscription tools might need to. When you pair this with powerful free models, it's a really cost-effective setup that prioritizes results.

Honestly, the specific tool matters, but the real driver is the underlying model. Getting unmitigated access to the best models (especially free ones!) and having a tool that leverages them effectively is key. Docs: https://docs.cline.bot

---

## Thread: What AI coding setup do you use? Cursor, Windsurf, VS Code with CLI tools, Roo Coder, or something else? (r/vibecoding)
https://www.reddit.com/r/vibecoding/comments/1jvvo59/what_ai_coding_setup_do_you_use_cursor_windsurf/

**Short/Succinct Option:**

Hey, Nick from Cline here. If you’re into vibe coding, Cline in VS Code is worth a look. You get Plan/Act modes for mapping out your workflow, can use any model (Claude, Gemini, DeepSeek, local), and extend it with custom tools via MCP. It’s usage-based, so you’re only paying for what you use, and you get full control over context. It’s the only setup I’ve found that actually feels like working with a real agent, not just a fancy autocomplete.

**Longer/More Detailed Option:**

Full disclosure -- I work on Cline. But here's why I love using it for my own projects (usually VS Code + Cline):

*   Model Choice is King: I'm mostly running Gemini 2.5 Pro Exp via OpenRouter (free + amazing). Also watching OpenRouter's free Quesar Alpha/Optimus stealth models. Cline lets you use any model, which is crucial because the model itself drives most of the magic.
*   MCP Servers Add Superpowers: Beyond the core coding, I use MCP servers all the time -- Perplexity for research, Firecrawl for web scraping, plus custom ones I built. Cline makes building these surprisingly easy (seriously, just give it API docs). Check out the MCP Marketplace too.
*   Plan/Act for Real Work: The Plan/Act flow feels natural for actually building stuff, much better than just endless chat prompts. Plan the attack, then let the agent execute.
*   Usage-Based = Unfiltered Power: Since you pay for tokens, Cline doesn't seem to nerf the model or context to fit a subscription budget. This is huge when you can leverage powerful free models like Gemini 2.5 or the Quesar ones. You get raw access.

Ultimately, the best setup gives you direct access to the best models without limitations. The tool should facilitate that, not get in the way. Docs: https://docs.cline.bot

---

## Thread: Is Vibe Coding a threat to Software Engineers in the private sector?
https://www.reddit.com/r/ChatGPTCoding/comments/1jw44ya/is_vibe_coding_a_threat_to_software_engineers_in/

**Short/Succinct Option:**

The real story isn’t that AI-powered “vibe coders” will wipe out software engineering jobs. If you look at what happens when you 5x the output of every engineer, the total demand for software actually explodes. History shows that when you make something dramatically cheaper and faster to produce, you don’t just replace old jobs—you unlock a ton of new use cases and markets that were never viable before. So yeah, the bar for “basic” work gets higher, but the pie gets way bigger. The real threat is missing the boat on these new opportunities, not being replaced by Fiverr gigs.

**Longer/More Detailed Option:**

This is a classic case of the Jevons Paradox in action. When you 5x engineering productivity with AI tools, you don’t just automate away jobs—you trigger a massive expansion in what gets built. Think about the textile revolution or the rise of semiconductors: as production got cheaper, demand skyrocketed, and whole new industries popped up. The same thing is happening with software. If you run the numbers, a 5x boost in developer output could add trillions to the global economy, not by replacing engineers, but by making it possible to build all the niche, hyperlocal, or “too small to matter” tools that never made sense before. Sure, the easy gigs get commoditized, but the real winners are the engineers and teams who learn to ride this new wave and solve problems nobody could touch before. If you’re curious about the economics, there’s a deep dive here: https://cline.bot/blog/what-happens-when-you-5x-the-output-of-every-engineer-unlocking-trillions-in-economic-value

---
