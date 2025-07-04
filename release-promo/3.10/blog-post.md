# Cline 3.10: Local Chrome Integration, YOLO Mode, Drag & Drop, and More Workflow Enhancements

Cline 3.10 is here, and it's packed with features designed to significantly enhance your development workflow, speed, and control. This release introduces a powerful new way to interact with the web, alongside several quality-of-life improvements and optimizations requested by the community. Let's dive in.

## Connect Cline to Your Local Chrome Browser

The headline feature of 3.10 is a fundamental shift in how Cline interacts with web content: you can now connect Cline directly to your running local Chrome browser instance via remote debugging.

Previously, Cline utilized a sessionless Chromium instance for browser tasks. While functional, this lacked the context of your active browsing sessions – your logins, cookies, and specific browser state. The new local Chrome integration changes everything. By enabling remote debugging on your Chrome instance and providing the port to Cline, you allow Cline to operate directly within your *real* browser environment.

This unlocks several powerful capabilities:

1.  **Seamless Debugging:** Point Cline at your locally running web application (`localhost:9222`, for example) and have it interact with elements, inspect network requests, or analyze console logs, all within the same browser session you're using for development. No more context switching or trying to replicate states in a separate headless instance.
    `[VIDEO: Chrome Use Case 1 - Debugging]`
2.  **Session-Based Automation:** Need Cline to interact with a service you're already logged into? Now it can. Cline can leverage your existing authenticated sessions in Chrome to perform tasks like summarizing private dashboards, drafting emails in your webmail client, interacting with project management tools, or even posting to social media on your behalf.
    `[VIDEO: Chrome Use Case 2 - Agentic Tasks]`
3.  **Accessing Private Content:** Extracting information from sites requiring login or navigating paywalls becomes straightforward. Cline can utilize your authenticated Chrome session to access and process content that was previously inaccessible to sessionless browsers.
    `[VIDEO: Chrome Use Case 3 - Private Content Extraction]`

This integration bridges the gap between automated tasks and the rich context of your personal browser environment, opening doors to more complex, stateful, and personalized agentic workflows than ever before. Imagine Cline helping you debug a complex UI issue by directly interacting with your dev tools, or summarizing meeting notes from your logged-in calendar app – it's now possible.

## Go Full Auto with YOLO Mode (Enable all commands)

For the power users who trust their process and want maximum speed, we've introduced the **"Enable all commands"** option, affectionately known as **YOLO Mode**. When enabled, this setting approves *ALL* actions requested by Cline – file edits, terminal commands, everything – without requiring individual confirmation.

This allows Cline to operate truly autonomously on a task until completion. Need to refactor a large chunk of code or run a complex sequence of build commands? Enable YOLO mode and let Cline handle it.

As the name implies, use this feature with extreme caution. Ensure you understand the task Cline is performing and have appropriate backups or version control in place, as Cline will proceed without interruption.
`[VIDEO: YOLO Mode]`

## New Task Tool

We've added a "New Task" tool: Cline can create new tasks using context from the current conversation, allowing you to maintain task flow while opening a new context window.

Try using `.clinerules` to suggest that Cline "start a new task when the context window is 50% full."

## Streamlined Workflow Enhancements

Beyond the major features, Cline 3.10 includes several other improvements to make your daily development smoother:

*   **Easy MCP Server Management:** A new modal accessible directly from the chat input area allows you to quickly view, enable, or disable your connected MCP servers without navigating deep into settings. Manage your available tools on the fly.
    `[VIDEO: MCP Modal]`
*   **Drag & Drop Context:** Simply drag files or entire folders directly onto the Cline chat interface (hold **Shift** while dragging) to add their contents or file structure as context for your task. Thanks to community member **eljapi** for this contribution!
    `[VIDEO: Drag and Drop]`
*   **CMD+' Shortcut:** Quickly add selected code or text from your editor directly into the Cline chat window using the `CMD+'` (Mac) / `Ctrl+'` (Win/Linux) keyboard shortcut. Streamline getting context into your prompts.
*   **Prompt Caching for LiteLLM + Claude:** Users leveraging LiteLLM with Claude models will now benefit from prompt caching, potentially reducing redundant token usage and speeding up repetitive requests. Thanks to community member **sammcj**!
*   **Smarter Context Management:** Cline now handles context more elegantly during long tasks. When the context window approaches 50% capacity, Cline automatically removes older, non-current versions of documents, keeping the focus on the most relevant information. This leads to better performance and less chance of looping.
*   **Reduced System Prompt Size:** We've optimized how Cline loads MCP documentation, dynamically fetching it only when needed. This significantly reduces the size of the initial system prompt, improving efficiency and potentially reducing token costs for certain operations.
*   **Fix: MCP Auto-Approve Sync:** Resolved an issue where the auto-approve toggle for specific MCP servers could become out of sync with the actual setting state.

## Get Started with Cline 3.10

This release represents a significant step forward in Cline's capabilities, particularly with the groundbreaking local Chrome integration. Update your Cline extension to version 3.10 today to explore these new features.

We're incredibly excited about the potential the local Chrome connection unlocks and can't wait to see the innovative workflows you build with it.

-   **Try it out:** Connect Cline to your local Chrome and experiment with debugging or automating tasks on your favorite websites.
-   **Share your feedback:** Let us know what you think! Join the discussion on our [Discord](<link-to-discord>) or [Reddit](<link-to-reddit>).
-   **Explore the docs:** Find more details on configuring the new features in the [Cline Documentation](<link-to-docs>).

Happy coding!
