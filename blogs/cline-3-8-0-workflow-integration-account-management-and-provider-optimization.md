# Cline 3.8.0: Workflow Integration, Account Management, and Provider Optimization

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

March 23, 2025 • 3 min read

*Here's what's new in 3.8.0:*

* **Streamlined workflows**: New 'Add to Cline' and 'Fix with Cline' code actions for faster problem-solving
* **Account view**: Track billing and usage history for Cline accounts directly in the extension
* **Sort underlying provider routing**: Choose how Cline routes API requests based on throughput, price, or latency to optimize for your specific needs
* **Rich MCP display improvements**: Visualize data more effectively with dynamic image loading and GIF support directly in your MCP chat output
* **Easy documentation access**: One-click access to Cline's documentation
* **Context window fix**: No more frustrating "Context Window Exceeded" errors when using OpenRouter or Cline Accounts
* **Disk space management**: See exactly how much storage Cline is using right next to the "Delete all Tasks" button in History view

## Streamlined Workflows with New Integration Points

### Add to Cline

0:00
/0:09

1×

Adding context to your Cline just got easier. With 3.8.0, we've added an 'Add to Cline' option when you right-click in a file or the terminal.

This new integration point allows you to quickly add important code snippets, error messages, or terminal output to your current Cline task without disrupting your workflow. Simply highlight text, right-click, and select 'Add to Cline' to provide your AI assistant with the context it needs to help you more effectively.

### Fix with Cline Code Actions

0:00
/0:08

1×

We've made fixing errors faster with the new 'Fix with Cline' code action. When you see a lightbulb icon in your editor, you can now select 'Fix with Cline' to send the code and associated errors directly to Cline for fixing.

For Cursor users, this feature is also accessible through the 'Quick Fix (CMD + .)' menu. This direct integration with VS Code's error handling system means you can address problems as soon as they appear, with Cline having all the context it needs to provide accurate solutions.

## Track Your Usage with the New Account View

0:00
/0:15

1×

No more tab-switching to check your Cline usage. With v3.8.0, we've integrated a full Account view directly into the extension.

The new Account view transforms how you manage your Cline usage by providing comprehensive visibility right where you need it. Now you can monitor billing and credit consumption, view your complete transaction history, and manage your account – all without leaving VS Code.

## Increased Control of Provider Routing Options

0:00
/0:15

1×

One of the most powerful additions in 3.8.0 is the new 'Sort underlying provider routing' setting. This feature gives you more control over how Cline and OpenRouter route your requests across different AI providers.

You can now optimize your experience based on what matters most to your specific project needs:

* **Throughput**: When processing power matters most, prioritize providers with the highest throughput capacity (like DeepSeek) for faster results
* **Price**: Working within budget constraints? Prioritize the lowest-cost providers for each request
* **Latency**: For real-time applications, minimize response times by prioritizing the providers with the lowest latency
* **Default**: Continue using our balanced approach that optimizes for both price and uptime

This granular control means no more compromises between cost and performance – simply adjust the routing strategy based on your current priorities.

## Enhanced Visual Context with Rich MCP Display

0:00
/0:10

1×

Cline 3.8.0 comes with improvements to the rich MCP display, now supporting dynamic image loading and GIF animation.

By bringing rich visual elements directly into your development workflow, Cline helps bridge the gap between text-based coding and visual understanding – making it more capable and your work more efficient.

## Quality of Life Improvements

Beyond the major feature additions, we've also addressed several important quality of life issues:

* **One-click documentation access**: We've added a 'Documentation' menu item to easily access Cline's docs whenever you need guidance
* **Improved cost reporting**: OpenRouter's new usage\_details feature provides more reliable cost tracking
* **Fixed "Context Window Exceeded" error**: Users of OpenRouter and Cline Accounts will no longer encounter this frustrating limitation, with additional context handling improvements coming soon
* **Better disk space management**: The History view now displays the total space Cline takes on disk right next to the "Delete all Tasks" button, giving you clear visibility into resource consumption
* **Enhanced MCP reliability**: Added a button to delete MCP servers in a failure state, preventing stuck processes
* **Bug fixes**: Fixed an issue where OpenRouter model ID could be set to an invalid value

*Cline 3.8.0 represents our ongoing commitment to creating a development assistant that integrates seamlessly into your workflow – not just helping you write code, but giving you the tools to manage resources, visualize data, and optimize performance.*

*Download the update now in VS Code and see how these improvements can enhance your development experience.*

*We're always eager to hear your feedback - let us know what you think of the new features and how we can make Cline even better for your workflow.*
