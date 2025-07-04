# Forget "Model Context Protocol" - Just Think of These as Extra Tools for Cline

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

February 22, 2025 • 3 min read

Yesterday, I asked a developer if he was using MCP in Cline.

"I still don't understand what Model Context Protocol is," he said.

I had to smile. Here was a developer missing out on powerful tools because he was getting caught up in confusing technical jargon. It's like developers are leaving features on the table because the name sounds too complicated.

"Forget Model Context Protocol - that's just distracting you from what matters," I told him. "Think of these as extra tools you can give to Cline. That's it."

You don't need to understand the technical architecture behind it, just like you don't need to understand the HTTP protocol to use a REST API. What matters is what these tools let you do: work seamlessly with your favorite services without constantly switching contexts and tabs.Let Me Show You What I Mean

Here's something you've probably done before:

**Without tools:**

> "Check what's in the latest PR"
>
> *switches to browser
>
> opens GitHub
>
> finds repository
>
> checks PR
>
> switches back to editor
>
> tries to remember what they were doing*

**With GitHub tools in Cline:**

> "Check what's in the latest PR"
>
> "The latest PR adds user authentication. Here are the main changes..."

Cline already knows which repository you're working in and what you're building. No context switching needed.

0:00
/0:12

1×

MCP Plugins give Cline access to context it didn't have before -- and Cline is smart enough to know WHEN and HOW to use these tools.

## These Tools Make Cline More Powerful

Think of Cline's capabilities like a toolbox:

* Out of the box, Cline can read files, write code, run commands, etc.
* But you can add more tools to help with specific tasks
* Each tool lets Cline do something new without you leaving your editor

## Why Context Matters: The Perplexity Example

This is where things get interesting. Let's say you're deep into building a feature and need to research something. Here's what usually happens:

Without tools, using Perplexity means:

1. Open a new tab
2. Go to Perplexity
3. Explain your ENTIRE project context again
4. "I'm working on a Next.js app with TypeScript, using Supabase for auth..."
5. Make your query
6. Come back to editor and paste in the result
7. Need another answer? Repeat the whole process

But when Perplexity is available as a tool for Cline, something magical happens. Cline already knows:

* What project you're working on
* Your tech stack
* Your current task
* Previous research you've done
* Your team's preferences

So when you ask a question, Cline can make a focused, contextual query to Perplexity without you having to re-explain everything. It's like having a senior developer who's been working on your project the whole time. Check it out here 👇

0:00
/0:23

1×

You shouldn't have to re-explain context when troubleshooting -- Cline is already aware.

## Here's What This Looks Like in Practice

Let's see a complete workflow in action when implementing authentication:

**Without tools:**

> "Implement Supabase user authentication"
>
> *opens Notion to check team standards
>
> searches through meeting notes
>
> opens Supabase docs in browser
>
> creates feature branch manually
>
> switches between windows constantly
>
> remembers to update Linear ticket*

**With tools in Cline:**

> "Implement Supabase user authentication"
>
> "I'll check our team's Notion first for our auth patterns..."
>
> "Found recent discussions about auth requirements in the team meetings..."
>
> "Let me research Supabase auth best practices..."
>
> "I'll create a feature branch and update the Linear ticket to track progress..."
>
> "Here's the implementation plan. Would you like me to proceed?"

Each step flows naturally into the next, with Cline maintaining context about your project, team preferences, and requirements throughout the entire process.

## What Tools Are Available?

Our marketplace has [hundreds of ready-to-use tools](https://cline.bot/mcp-marketplace?ref=cline.ghost.io). Here are some popular ones:

0:00
/1:13

1×

There are literally hundreds of tools available to you to add to Cline in our MCP Marketplace

Daily Development:

* GitHub for managing repositories and PRs
* Notion for checking team documentation
* Linear for tracking tasks

Research & Documentation:

* Perplexity Research for smart documentation search
* WolframAlpha for complex computations
* Supabase for database patterns

Debugging:

* Sentry for error tracking
* Raygun for crash reporting
* Kubernetes Observer for cluster monitoring

## "But Is This Complicated to Set Up?"

Nope. Most tools just need:

1. Click "Install" in Cline
2. Add an API key if the plugin needs one
3. That's it

0:00
/0:20

1×

Adding Plugins to Cline is pretty simple.

## Start Small

Pick ONE tool you use frequently - maybe GitHub or Notion (or Perplexity – my favorite). Add it to Cline and try it for a week.

You'll be surprised how quickly "let me switch to my browser" becomes "Cline, can you check that for me?"

---

*This blog was written by Nick Baumann, Product Marketing at Cline. Follow us*[*@cline*](https://twitter.com/cline?ref=cline.ghost.io)*for more insights into the future of development.*

[*Install Cline*](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev&ref=cline.ghost.io)

*Join our community:*[*Discord*](https://discord.gg/cline?ref=cline.ghost.io)*&*[*Reddit*](https://reddit.com/r/cline?ref=cline.ghost.io)
