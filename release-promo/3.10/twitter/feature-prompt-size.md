Smaller system prompts = faster responses & lower costs.

30% smaller system prompt
distracts models way less (for less powerful models)
reduces token usage
keeps model from being distracted from mcp-related instructions

In Cline 3.10, MCP server documentation is loaded dynamically when needed, instead of sitting in the system prompt. This saves context window space, tokens, and cost, especially with many tools enabled.

`[VISUAL: Prompt Size Comparison Before/After]`
