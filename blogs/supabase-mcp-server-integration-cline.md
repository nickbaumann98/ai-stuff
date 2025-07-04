# Finally: Manage Your Supabase Database Directly From Cline

For developers using Cline, the gap between AI-assisted coding and direct database management just closed. We've heard the requests, and it's finally here: the official **Supabase MCP Server** is now live in the Cline MCP Marketplace. This is a significant milestone, marking the first time a major database platform like Supabase has full read *and* write access enabled through an official MCP server, directly usable within your AI development workflow.

No more context switching between your editor, the Supabase dashboard, and SQL clients. You can now interact with your database – execute queries, manage schemas, fetch configurations, and more – all orchestrated by Cline, right where you code.

**[INSERT VIDEO: supabase-execute-sql.mp4]**
Imagine asking Cline to fetch specific user data or update a record, and watching it execute the SQL query directly against your Supabase instance. That's the power now available.

## Bridging AI and Your Backend (Information)

The Model Context Protocol (MCP) acts as a standardized bridge, allowing AI agents like Cline to securely interact with external tools and services. The Supabase MCP server leverages this protocol to provide Cline with over 20 distinct "tools" or capabilities for database interaction.

This isn't just about reading data; it's about empowering Cline to actively participate in the full development lifecycle of your backend.

## Getting Started: Setup in Minutes (Information/Desire)

Integrating this powerful capability is straightforward:

1.  **Generate a Supabase PAT:** First, you need a Personal Access Token (PAT) from Supabase for authentication. This ensures secure access tied to your account. You can generate one here: [supabase.com/dashboard/account/tokens](https://supabase.com/dashboard/account/tokens)
2.  **Install from Cline Marketplace:** Open Cline in VS Code/Cursor, navigate to the MCP Marketplace (Extensions -> Cline -> MCP Marketplace), find the official Supabase server, and click "Install".
3.  **Enter Your PAT:** During installation, Cline will prompt you to securely enter the Supabase PAT you generated.

That's it. Cline is now connected to your Supabase account.

## What Can You Do? Key Capabilities (Information/Desire)

With the Supabase MCP server installed, you can delegate numerous database tasks to Cline:

*   **Direct SQL Execution:** Run `SELECT`, `INSERT`, `UPDATE`, `DELETE` queries using the `execute_sql` tool. Perfect for quick data checks or manipulations.
    **[INSERT VIDEO: supabase-execute-sql.mp4]**
*   **Schema Management via Migrations:** Ask Cline to create or alter tables, or even define entire schemas. It will generate the appropriate DDL and apply it using the `apply_migration` tool, keeping your schema changes tracked.
    **[INSERT VIDEO: supabase-create-table.mp4]**
    **[INSERT VIDEO: supabase-edit-table.mp4]**
    **[INSERT VIDEO: supabase-create-schema.mp4]**
*   **Configuration Fetching:** Need your project URL or anon key? Use `get_project_url` and `get_anon_key`.
*   **Type Generation:** Keep your frontend types in sync with your database schema using `generate_typescript_types`.
*   **Debugging:** Pull recent logs directly into your editor for troubleshooting with `get_logs`.
*   **Database Branching (Experimental):** Manage Supabase's new branching features (`create_branch`, `list_branches`, `merge_branch`) for safer development workflows.

This integration streamlines common database operations, allowing you to stay focused within your development environment and leverage AI for tasks that previously required manual intervention and context switching.

## The Future is Conversational (Desire)

This integration represents more than just convenience; it points towards a future where interacting with complex backend systems becomes a conversation. By bridging the gap between natural language intent and database actions, we're making powerful tools like Supabase more accessible and enabling truly AI-driven development workflows.

Developers have been asking for this level of integration, and we're thrilled to deliver it alongside the Supabase team.

## Get Started Today (Action)

Ready to stop switching tabs and start managing Supabase directly from Cline?

1.  **Install Cline** if you haven't already: [Link to Cline website/download]
2.  **Install the Supabase MCP Server** from the MCP Marketplace within Cline.
3.  **Explore the possibilities:** Ask Cline to interact with your Supabase project.
4.  **Share your feedback:** Let us know what you build and what other integrations you'd like to see in the [Cline Discord](<Your Discord Link Here>) or on [GitHub](https://github.com/supabase-community/supabase-mcp/issues).

Learn more about the integration on the Supabase blog: [supabase.com/blog/mcp-server](https://supabase.com/blog/mcp-server)
