# Memory Bank: How to Make Cline an AI Agent That Never Forgets

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

February 6, 2025 • 4 min read

Imagine a detective who loses his memory every time he falls asleep. To solve cases, he develops an ingenious system: tattooing critical facts on his body and keeping a carefully organized set of Polaroid photos. Each time he wakes up, he can quickly rebuild his understanding by following his own documentation system. That's the plot of Memento, and it inspired how we solved a common problem with AI coding assistants.

[Dont Believe His Lies Memento GIF](https://tenor.com/view/dont-believe-his-lies-memento-gif-11382090?ref=cline.ghost.io)from [Dont Believe His Lies GIFs](https://tenor.com/search/dont%2Bbelieve%2Bhis%2Blies-gifs?ref=cline.ghost.io)

Here's the thing about AI assistants like Cline: they're brilliant but forgetful. Every time you start a new chat, your context window fills up or resets, forcing you to waste precious minutes re-explaining your project, tech stack, and architecture. It's like working with a genius who gets amnesia every coffee break.

But what if we could turn this limitation into a strength?

## How [Memory Bank](https://docs.cline.bot/improving-your-prompting-skills/custom-instructions-library/cline-memory-bank?ref=cline.ghost.io) Works

Memory Bank is a community-created custom instruction set for Cline. When you add these instructions to Cline's settings, you're essentially telling it:

> "Before you do any work, check the memory-bank/ folder in the project. If those files don't exist, create them. If they do exist, read them to understand the project context."

The system uses a combination of markdown files for documentation and Mermaid diagrams in the instructions themselves to teach Cline how to maintain this documentation structure. When Cline's context window fills up or a new session starts, it can quickly rebuild its understanding by reading these files - just like Memento's protagonist checking his notes.

0:00
/1:12

1×

## Understanding Context Windows and Memory in AI Systems

Before we dive deeper into the Memory Bank, it's important to understand why this solution is so crucial. AI assistants like Cline operate with what we call a "[context window](https://cline.bot/blog/understanding-the-new-context-window-progress-bar-in-cline?ref=cline.ghost.io)" – essentially the amount of conversation and code they can "remember" at once. This window is finite, typically ranging from 32k to 200k tokens depending on the model.

When you're working on a complex project, you'll inevitably hit this limit. Traditional solutions include:

1. Starting a new chat (losing all context)
2. Carefully managing what you include in each prompt
3. Using summarization techniques to compress context

None of these are ideal. They either sacrifice important context or require constant manual management. The Memory Bank system offers a different approach entirely.

## The Architecture of Memory

Memory Bank works on two levels. The custom instructions utilize Mermaid diagrams to tell Cline how to manage documentation:

```
flowchart TD
    PB[projectbrief.md] --> PC[productContext.md]
    PB --> SP[systemPatterns.md]
    PB --> TC[techContext.md]

    PC --> AC[activeContext.md]
    SP --> AC
    TC --> AC

    AC --> P[progress.md]

```
> The above Mermaid diagram code rendered visually 👇

![](https://cline.ghost.io/content/images/2025/02/image-13.png)

In this case, projectbrief.md is the source of truth from which other docs come from

This diagram isn't just for show – it's actually part of the [custom instructions](https://docs.cline.bot/improving-your-prompting-skills/custom-instructions-library/cline-memory-bank?ref=cline.ghost.io) that tell Cline how the documentation system should work. The actual documentation itself is then created in simple markdown files, following the structure that the diagram defines.

It's a clever approach: use visual flowcharts to teach the AI how to maintain text documentation. The Mermaid diagram provides the "rules," and the markdown files hold the actual project knowledge.

### Core Files

1. **projectbrief.md**: The foundation document that shapes everything else
2. **productContext.md**: The business and user perspective
3. **systemPatterns.md**: Technical architecture and decisions
4. **techContext.md**: Development environment and stack
5. **activeContext.md**: Current state of development
6. **progress.md**: Project status and tracking

0:00
/0:14

1×

## Digging Deeping: The Memory Bank Lifecycle

The Memory Bank operates on a continuous cycle of read, verify, execute, and update. Here's a detailed look at how it works:

![](https://cline.ghost.io/content/images/2025/02/image-12.png)

The above code can be rendered as this Mermaid Diagram

### Initial Setup

When starting a new project:

1. Cline creates the `memory-bank/` directory
2. Initializes all required files
3. Requests necessary information from users
4. Establishes baseline documentation

### During Development

Before any work:

1. Read all Memory Bank files
2. Verify context is complete

During work:

1. Follow established patterns
2. Track changes and decisions
3. Monitor context window usage

After significant changes:

1. Update relevant documentation
2. Ensure consistency across files
3. Prepare for potential context resets

## Visual Prompting: Guiding AI with Flowcharts

![](https://cline.ghost.io/content/images/2025/02/image-15.png)

Standing wisdom is to write system prompts in markdown, JSON, or [XML](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/use-xml-tags?ref=cline.ghost.io). However, our community has found Mermaid diagrams (which Claude is quite adept at creating) to be useful for prompting.

Instead of writing process instructions markdown, they use write in flowcharts like this:

```
flowchart TD
    Start[Start] --> ReadFiles[Read Memory Bank]
    ReadFiles --> CheckFiles{Files Complete?}

    CheckFiles -->|No| Plan[Create Plan]
    Plan --> Document[Document in Chat]

    CheckFiles -->|Yes| Verify[Verify Context]
    Verify --> Strategy[Develop Strategy]
    Strategy --> Present[Present Approach]

```

Here's why this matters: Mermaid diagrams aren't just prettier than text – they're a formal language for describing workflows. Each node, connection, and decision point is explicitly defined. For an AI, this structured format might actually be easier to understand than paragraphs of natural language trying to describe the same process.

When we write text instructions, there's room for ambiguity. But a flowchart in Mermaid code is unambiguous – each state and transition is clearly defined. It's like giving the AI a precise map instead of vague directions.

The full Memory Bank instructions are in the [Cline documentation](https://docs.cline.bot/improving-your-prompting-skills/custom-instructions-library/cline-memory-bank?ref=cline.ghost.io). But the bigger insight is that maybe we should be thinking more about how AI actually processes information. Sometimes the best way to communicate with AI isn't through natural language – it's through the structured language of workflows.

---

*This blog was written by Nick Baumann, Product Marketing at Cline. Follow us*[*@cline*](https://twitter.com/cline?ref=cline.ghost.io)*for more insights into the future of development.*

[*Install Cline*](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev&ref=cline.ghost.io)

*Join our community:*[*Discord*](https://discord.gg/cline?ref=cline.ghost.io)*&*[*Reddit*](https://reddit.com/r/cline?ref=cline.ghost.io)
