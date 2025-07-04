# SICP Revisited: Writing Code for People *and* AI Agents

Since SICP, it's been a maxim of software engineering that "Programs must be written for people to read, and only incidentally for machines to execute." However, in the age of generative AI, code is increasingly often read by agents as well. As generative AI tools become popular, it's important that we as engineering leaders better understand how agents interpret the code we maintain.

## Understanding AI's Current Limitations

Agents currently do not maintain a long-term understanding of our codebases. Every experience is like learning it for the first time again. Using common patterns and best practices becomes increasingly important as it better reflects their training set. The degree you stray from this will degrade the effectiveness of your agent.

The context window is also a precious resource. It's best to keep files short in length as repeated I/O to lengthy files can quickly consume the available context, forcing the agent to make difficult decisions about what information to retain or discard, often leading to degraded performance.

## The Challenge of Abstraction and Decoupling

As it stands, highly decoupled and abstracted systems can be difficult for agents to understand since it requires any change to be spread across several files. For example, a typical API might have handler, service, repository, and migration layers, as well as cross-cutting concerns like custom error handling, validation, logging, and tracing. This fragmentation can make it harder for AI tools to understand the complete picture and provide accurate assistance.

## Adapting for the Future of AI Collaboration

Generative coding platforms will soon have the capacity to tackle this level of complexity with more sophisticated strategies for prompting and context management. However, in the meantime, I encourage you to start evaluating your codebase through the lens of AI readability. Consider how your architectural decisions might impact the effectiveness of AI-assisted development. Try using tools like Cline to experience firsthand how AI agents interact with your code, and begin optimizing your development practices for this new era of collaborative coding.

Remember: The goal isn't to compromise on code quality or engineering principles, but to evolve our practices to accommodate both human and AI readers effectively. The future of software development will likely be a partnership between human creativity and AI assistance - let's make sure our code is ready for it.
