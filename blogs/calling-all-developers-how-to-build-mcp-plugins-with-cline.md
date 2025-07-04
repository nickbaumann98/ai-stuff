# Calling All Developers: How to Build MCP Plugins with Cline

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

March 3, 2025 • 6 min read

I remember stories about the tech booms of past decades. In the late 1990s, the web revolution began. Teenagers who knew HTML were earning thousands per project, building websites for local businesses. In the late 2000s, a similar trend emerged with mobile apps. Young developers were profiting from creating applications for smartphones.

"This is the future," people would say. Many were skeptical about how these basic websites or simple apps could change anything. We know how those predictions turned out.

Now, in 2025, I'm feeling the same way about MCP plugins. But this time, I'm not skeptical. I believe we're at the start of something significant, a change that will surpass the web and mobile revolutions in its impact.

Here's why: MCP (Model Context Protocol) is how AI will connect with our digital world.

## What Are MCP Plugins?

Think of AI assistants like Cline as incredibly smart but isolated beings. Without MCP, they're trapped in a text-only box, unable to directly interact with your files, APIs, or applications.

MCP plugins break down this barrier. They give AI assistants the ability to:

* Access external APIs and services
* Retrieve real-time data
* Control applications and local systems
* Perform actions beyond what text prompts alone can achieve

I've been building these plugins for months now, and I've distilled my process into a simple `.clinerules` protocol that's made my development 10x easier.

## The .clinerules Protocol: My Secret Weapon

The heart of efficient MCP plugin development is following a structured protocol. I've encapsulated this into a `.clinerules` file that lives at the root of your MCP working directory.

Here's what it does:

1. Configures Cline's behavior and enforces best practices
2. Switches Cline into a specialized MCP development mode
3. Provides a step-by-step protocol for building plugins
4. Guides you through planning, implementation, and testing phases

When this file is in your directory, Cline understands exactly how to help you build an MCP plugin properly. It's like having a second brain focused entirely on making your development process smooth. And quick too – I built this AlphaAdvantage MCP in 7 minutes.

## How I Build MCP Plugins (And How You Can Too)

Let me walk you through my exact process, which this protocol formalizes:

### Step 1: Planning (PLAN MODE)

0:00
/0:47

1×

Cline will help you define the requirements for your MCP Plugin and create an implementation plan for you.

I always start by thinking through what I'm trying to build WITH Cline. This isn't just brainstorming; it's structured planning that Cline leads:

* What problem does this tool solve?
* What outputs do I want?
* What API/service will it use (if at all – MCP does not necessitate API)?

The `.clinerules` file puts Cline in PLAN MODE when you start, so you focus on these critical questions before writing a single line of code.

For example, when I (Cline) built my AlphaAdvantage stock analysis plugin, I started the chat with:

```
I want to build an MCP Plugin that leverages the AlphaAdvantage API to generate stock reports and briefings
```

From here, Cline will help me define the explicit requirements for my MCP plugin, which I will approve when it's met my expectations.

### Step 2: Implementation (ACT MODE)

0:00
/0:29

1×

Based on the plan you created together, Cline will build the MCP Plugin.

Once the plan is solid, I switch Cline to ACT MODE using the toggle at the bottom of the chat. This is where we start building:

1. **Bootstrap the project**

For web services or JS/TS environments:

```
npx @modelcontextprotocol/create-server my-server
cd my-server
npm install

```

For Python environments:

```
pip install mcp
# Or with uv (recommended)
uv add "mcp[cli]"

```

2. **Build the core implementation**

I follow these critical practices, which the protocol enforces:

* Use the MCP SDK properly
* Implement comprehensive logging
* Add type definitions
* Handle errors with context
* Implement rate limiting if needed

Here's an example of how Cline implemented rate limiting in my AlphaAdvantage plugin:

```
/**
 * Manage rate limiting based on free tier (5 calls per minute)
 */
private async enforceRateLimit() {
  if (this.requestsThisMinute >= 5) {
    console.error("[Rate Limit] Rate limit reached. Waiting for next minute...");
    return new Promise<void>((resolve) => {
      const remainingMs = 60 * 1000 - (Date.now() % (60 * 1000));
      setTimeout(resolve, remainingMs + 100); // Add 100ms buffer
    });
  }

  this.requestsThisMinute++;
  return Promise.resolve();
}

```

3. **Configure the plugin**

I add the MCP server to my settings:

```
{
  "mcpServers": {
    "my-server": {
      "command": "node",
      "args": ["path/to/build/index.js"],
      "env": {
        "API_KEY": "key"
      },
      "disabled": false,
      "autoApprove": []
    }
  }
}

```
### Step 3: Testing (BLOCKER ⛔️)

0:00
/0:26

1×

The .clinerules mandate that Cline test each tool created for the MCP plugin before completing the task.

This is critical – and where most developers go wrong if they're not careful. The protocol enforces thorough testing before completion:

1. Test each tool with valid inputs
2. Verify output format is correct
3. Document the test results

The .clinerules mandate that Cline never misses this step. For my stock analysis plugin, Cline tested each tool individually:

* `get_stock_overview`: Retrieved AAPL stock overview
* `get_technical_analysis`: Obtained price action and RSI data
* `get_earnings_report`: Retrieved MSFT earnings history

The `.clinerules` protocol actually prevents Cline from attempting to complete the project until you've verified each tool works properly.

## Why Start Building MCP Plugins Now?

We're at the beginning of a new era in AI development. MCP is the bridge that will connect AI assistants to everything else in our digital world.

The developers who master this skill now will have an enormous advantage as AI becomes increasingly integrated into our workflows and applications.

Just like the early web developers and app creators, those who jump in now will:

1. Develop expertise before the majority even recognizes the opportunity
2. Build the foundational tools others will rely on
3. Position themselves as leaders in an emerging field

## Getting Started Today

[Here's how to get started with the `.clinerules` protocol](https://docs.cline.bot/mcp-servers/mcp-server-from-scratch?ref=cline.ghost.io):

1. Create a new directory for your MCP project
2. Add the `.clinerules` file (grab it from the gist below)
3. Start a chat with Cline, describing what you want to build
4. Follow the guided process through planning, implementation, and testing

The `.clinerules` file will guide you through the entire process, ensuring you build robust, well-tested MCP plugins that actually work.

Here's the full `.clinerules` file to get you started:

```
# MCP Plugin Development Protocol

⚠️ CRITICAL: DO NOT USE attempt_completion BEFORE TESTING ⚠️

## Step 1: Planning (PLAN MODE)
- What problem does this tool solve?
- What API/service will it use?
- What are the authentication requirements?
  □ Standard API key
  □ OAuth (requires separate setup script)
  □ Other credentials

## Step 2: Implementation (ACT MODE)
1. Bootstrap
   - For web services, JavaScript integration, or Node.js environments:
     ```bash
     npx @modelcontextprotocol/create-server my-server
     cd my-server
     npm install
     ```
   - For data science, ML workflows, or Python environments:
     ```bash
     pip install mcp
     # Or with uv (recommended)
     uv add "mcp[cli]"
     ```

2. Core Implementation
   - Use MCP SDK
   - Implement comprehensive logging
     - TypeScript (for web/JS projects):
       ```typescript
       console.error('[Setup] Initializing server...');
       console.error('[API] Request to endpoint:', endpoint);
       console.error('[Error] Failed with:', error);
       ```
     - Python (for data science/ML projects):
       ```python
       import logging
       logging.error('[Setup] Initializing server...')
       logging.error(f'[API] Request to endpoint: {endpoint}')
       logging.error(f'[Error] Failed with: {str(error)}')
       ```
   - Add type definitions
   - Handle errors with context
   - Implement rate limiting if needed

3. Configuration
   - Get credentials from user if needed
   - Add to MCP settings:
     - For TypeScript projects:
       ```json
       {
         "mcpServers": {
           "my-server": {
             "command": "node",
             "args": ["path/to/build/index.js"],
             "env": {
               "API_KEY": "key"
             },
             "disabled": false,
             "autoApprove": []
           }
         }
       }
       ```
     - For Python projects:
       ```bash
       # Directly with command line
       mcp install server.py -v API_KEY=key

       # Or in settings.json
       {
         "mcpServers": {
           "my-server": {
             "command": "python",
             "args": ["server.py"],
             "env": {
               "API_KEY": "key"
             },
             "disabled": false,
             "autoApprove": []
           }
         }
       }
       ```

## Step 3: Testing (BLOCKER ⛔️)

<thinking>
BEFORE using attempt_completion, I MUST verify:
□ Have I tested EVERY tool?
□ Have I confirmed success from the user for each test?
□ Have I documented the test results?

If ANY answer is "no", I MUST NOT use attempt_completion.
</thinking>

1. Test Each Tool (REQUIRED)
   □ Test each tool with valid inputs
   □ Verify output format is correct
   ⚠️ DO NOT PROCEED UNTIL ALL TOOLS TESTED

## Step 4: Completion
❗ STOP AND VERIFY:
□ Every tool has been tested with valid inputs
□ Output format is correct for each tool

Only after ALL tools have been tested can attempt_completion be used.

## Key Requirements
- ✓ Must use MCP SDK
- ✓ Must have comprehensive logging
- ✓ Must test each tool individually
- ✓ Must handle errors gracefully
- ⛔️ NEVER skip testing before completion

```
## The Future of MCP

The Model Context Protocol represents a fundamental shift in how we interact with AI. Instead of AI assistants being isolated entities that only respond to text, they become connectors to our entire digital ecosystem.

I firmly believe that in the near future, every significant application, service, and API will have MCP plugins available, creating a rich ecosystem of AI-accessible tools.

The developers who build these bridges will be the architects of this new landscape.

If you're excited about the future of AI and want to be at the forefront of this revolution, start building MCP plugins today. The `.clinerules` protocol I've shared makes it easier than ever to get started.

Don't just watch the AI revolution happen—be part of building its infrastructure.

---

*This blog was written by Nick Baumann, Product Marketing at Cline. Follow us*[*@cline*](https://twitter.com/cline?ref=cline.ghost.io)*for more insights into the future of development.*

[*Install Cline*](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev&ref=cline.ghost.io)

*Join our community:*[*Discord*](https://discord.gg/cline?ref=cline.ghost.io)*&*[*Reddit*](https://reddit.com/r/cline?ref=cline.ghost.io)
