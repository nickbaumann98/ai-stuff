# How Cline Handles Context Engineering for You

Karpathy's right: "context engineering" > "prompt engineering." While others debate terminology, we've been quietly solving the hardest part -- making context engineering invisible. Here's how Cline handles it for you:

Modern AI models don't need clever prompts. They need the right information at the right time. Give them relevant code, file structures, and past decisions -- they'll figure out what to do. The challenge is managing what information the model sees and when.

## The Problem

You know the pain. Deep in a complex task, the AI understands everything perfectly, then -- context window full. The AI forgets. You start over.

Manual context management means constantly deciding what to keep, what to delete. It's janitorial work, not coding.

## Cline's Automatic Solution

Cline manages context like a skilled editor. Here's how:

**Smart Compression.** Before deleting anything, Cline finds redundancies. Read the same file three times? It keeps only the latest version, replacing older ones with a note. This often frees thousands of tokens without losing conversation flow.

**Surgical Cuts.** When compression isn't enough, Cline preserves what matters: your original task and recent messages. It cuts from the middle -- the least relevant part. Everything's tracked in a non-destructive log, so nothing's truly lost.

**Reactive Approach.** No constant overhead. Cline waits until you're near limits, then acts. Efficient and predictable.

## Manual Control Options

Sometimes you need to take the wheel:

- **`/newtask`**: Archive current work and start fresh with a clean context
- **Manual edits**: Delete irrelevant blocks yourself
- **Context bar**: Visual indicator shows usage -- start fresh at 70-80% if needed

## Why It Matters

This is the "thick layer of non-trivial software" Karpathy mentions. It's the difference between an AI that constantly forgets and one that maintains understanding across hours of work.

The best part? It's invisible. While others manage conversation history manually, you're shipping code.

Stop managing windows. Start building software.

[Download Cline](https://github.com/cline/cline) | [Join the Discussion](https://www.reddit.com/r/cline/)
