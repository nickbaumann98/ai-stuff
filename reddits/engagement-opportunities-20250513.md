# Reddit Engagement Opportunities - 2025-05-13

## Thread 1: Planning is what actually improves output when building with AI
Link: https://www.reddit.com/r/ChatGPTCoding/comments/1klruq3/planning_is_what_actually_improves_output_when/

**Draft Option (Longer & More Detailed):**
This is spot on. It's so tempting to just dive in when AI makes iteration feel fast, but without a solid plan, you often end up going in circles or building something that doesn't quite hit the mark.

We've found this to be so critical that we designed Cline with distinct Plan and Act modes. The whole idea of Plan Mode is to have that upfront collaborative session with the AI. You define the task, let Cline explore the codebase using its tools to build understanding, discuss constraints, and align on a strategy. It's like briefing a skilled developer before they start coding.

Then, when you toggle to Act Mode, Cline is executing a mission it's been thoroughly prepped for. The actions are way more precise and aligned with the project's needs because of that shared understanding built during planning. It's a bit more upfront effort, but it pays off massively in speed and quality down the line. We even wrote a bit about our thinking here if you're interested: https://docs.cline.bot/exploring-clines-tools/plan-and-act-modes-a-guide-to-effective-ai-development

---

## Thread 2: Things you don't like in Cursor/ Features you'd want in Cursor
Link: https://www.reddit.com/r/ChatGPTCoding/comments/1km01p4/things_you_dont_like_in_cursor_features_youd_want/

**Draft Option (Longer & More Detailed):**
Hey, Nick from Cline here. It's interesting to see discussions about what developers are looking for beyond current tools like Cursor.

If you're exploring, Cline offers a different approach. It's also in VS Code but functions more as an agent. Some things users appreciate are:

- Plan/Act Workflow: Instead of just chat, Cline has a Plan Mode where you and the AI define the task, explore the codebase, and agree on a strategy. Then Act Mode executes that plan with your approval. This gives more control and often leads to better, more precise results, especially for complex tasks.
- Bring-Your-Own-Key (BYOK) Model: You're not tied to a specific LLM or subscription. You use your own API keys (OpenAI, Anthropic, Google, local models via Ollama, etc.). This means you can pick the best model for the job (e.g., Gemini 2.5 Pro for coding, Claude 3.7 for reasoning) and only pay for what you use.
- Extensibility via MCP (Model Context Protocol): This is a big one. MCP allows Cline to use a growing ecosystem of external tools and services (MCP servers). Think specialized tools for web scraping (Firecrawl), research (Perplexity), interacting with APIs (GitHub, Supabase), or even custom tools you build yourself. The MCP Marketplace makes these easy to discover and install. This makes Cline highly adaptable.
- Checkpoints: Easily revert changes if something doesn't go as planned.

While Cline itself isn't open source, the MCP ecosystem encourages open-source contributions for servers, and we're focused on building a flexible, powerful agent that integrates well with a developer's existing toolkit. Might be worth a look if those aspects resonate with what you're looking for. You can find more info at https://docs.cline.bot.

---

## Thread 3: What’s an underrated use of AI that’s saved you serious time?
Link: https://www.reddit.com/r/ChatGPTCoding/comments/1klk97f/whats_an_underrated_use_of_ai_thats_saved_you/

**Draft Option (Longer & More Detailed):**
That's a great point about voice-to-text! I've had a similar experience. One of the biggest underrated time-savers for me has been using voice input directly with my coding assistant.

I use Aqua Voice integrated with Cline, and the efficiency boost is pretty noticeable. Instead of meticulously typing out detailed prompts, instructions for refactoring, or even just brainstorming ideas, I can just say it. It's especially useful when you're trying to explain a complex thought or a multi-step process to the AI – speaking it out loud is often much quicker and more natural than translating it into precise text. It really cuts down on the friction and helps maintain focus. Definitely faster than typing for a lot of interactions.

---
