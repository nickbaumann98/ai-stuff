# Cline 3.17.9: Experimental Claude 4 Support + Task Timeline Navigation

Just dropped v3.17.9 with some solid improvements, especially for Claude 4 users who've been dealing with edit failures.

## What's New

**Claude 4 Reliability Fixes (Experimental)**

If you've been using Claude 4 with Cline, you know the pain -- edit failures, fallbacks to full file rewrites, general frustration. We've made experimental changes to how Cline communicates with Claude 4, specifically around search/replace operations. Swapped out some delimiters (< and > with - and +) which is showing much better results in testing.

Shoutout to @heguro for inspiring this approach with their original suggestion and commit!

[VIDEO: Claude 4 Improved Edit Success Rate]

This is still experimental, so we're looking for feedback. Try Claude 4 as your daily driver for a few days and let us know how it compares to Claude 3.7 or Gemini.

**Task Timeline Scrolling**

New feature that lets you click any point in your task timeline and jump directly to that moment in the conversation. Super useful when you need to understand context behind a code change or want to branch from an earlier point.

[VIDEO: Task Timeline Navigation Demo]

**CSV/XLSX File Support**

You can now drag and drop spreadsheets directly into Cline for analysis. CSV files work great, and basic Excel files are supported. For complex Excel files with advanced features, Cline can generate Python scripts to handle the processing. Good foundation for data analysis workflows.

## Other Improvements

- New Grok-3 models from xAI (grok-3, grok-3-fast, grok-3-mini, grok-3-mini-fast) (Thanks @PeterDaveHello!)
- Fixed AWS Bedrock credential caching issues (Thanks @DaveFres!)
- Better search tool behavior (was overloading conversations with massive outputs)
- Checkpoint system fixes
- Improved chat box UI

## Community Shoutouts

Thanks to all our community contributors who made this release possible through bug reports, feature requests, and code contributions!

## Testing Help Needed

Since the Claude 4 improvements are experimental, we really want community feedback before making it our default recommendation. Test it on:

- Long code files with complex diff editing
- Multiple search/replace operations  
- General vibe check vs Claude 3.7/Gemini

Use /reportbug in chat if you hit any issues.

Available now on VS Code, Cursor, and Windsurf marketplaces.

Docs: https://docs.cline.bot
Discord: https://discord.gg/cline
Changelog: https://github.com/cline/cline/blob/main/CHANGELOG.md
