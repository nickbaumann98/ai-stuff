# Cline v3.15.0: Release Promo Plan Overview

**Version:** 3.15.0
**Date:** May 10, 2025
**Objective:** To outline the strategy, key messages, and content plan for promoting the Cline v3.15.0 release, ensuring alignment with Cline's core principles and maximizing community engagement.

# Changelog

## [3.15.0]

-   Add Task Timeline visualization to tasks (Thanks eomcaleb!)
-   Add cache to ui for OpenAi provider
-   Add FeatureFlagProvider service for the Node.js extension side
-   Add copy buttons to task header and assistant messages
-   Add a more simplified home header was added
-   Add ability to favorite a task, allowing it to be kept when clearing all tasks
-   Add npm script for issue creation (Thanks DaveFres!)
-   Add confirmation dialog to Delete All History button
-   Add ability to allow the user to type their next message into the chat while Cline is taking action
-   Add ability to generate commit message via cline (Thanks zapp88!)
-   Add improvements to caching for gemini models on OpenRouter and Cline providers
-   Add improvements to allow scrolling the file being edited.
-   Add ui for windsurf and cursor rules
-   Add mistral medium-3 model
-   Add option to collect events to send them in a bundle to avoid sending too many events
-   Add support to quote a previous message in chat
-   Add support for Gemini Implicit Caching
-   Add support for batch selection and deletion of tasks in history (Thanks danix800!)
-   Update change suggested models
-   Update fetch cache details from generation endpoint
-   Update converted docs to Mintlify
-   Update the isOminiModel to include o4-mini model (Thanks PeterDaveHello!)
-   Update file size that can be read by Cline, allowing larger files
-   Update defaults for bedrock API models (Thanks Watany!)
-   Update to extend ReasoningEffort to non-o3-mini reasoning models for all providers (Thanks PeterDaveHello!)
-   Update to give error when a user tries to upload an image larger than 7500x7500 pixels
-   Update announcement so that previous updates are in a dropdown
-   Update UI for auto approve with favorited settings
-   Fix bug where certain terminal commands would lock you out of a task
-   Fix only initialize posthog in the webview if the user has opted into telemetry
-   Fix bug where autocapture was on for front-end telemetry
-   Fix for markdown copy excessively escaping characters (Thanks weshoke!)
-   Fix an issue where loading never finished when using an application inference profile for the model ID (Thanks WinterYukky!)

## 1. Overall Release Theme & Key Message

**Core Theme:** "Cline v3.15: Deeper Insights, Seamless Workflow, and Empowered Community."
This theme emphasizes the key advancements: understanding agentic processes better (Task Timeline), smoother user experience (Non-Blocking UI, Terminal Fixes), and stronger community involvement (New Docs).

**Key Message:** Cline v3.15 delivers a significantly more intuitive, responsive, and transparent agentic coding experience. With groundbreaking features like the Task Timeline for unprecedented insight, seamless Gemini 2.5 Pro caching for cost efficiency, a revamped community-driven documentation platform, and crucial UX enhancements that keep you in the flow, Cline continues to solidify its position as the most powerful and principled AI coding partner for developers.

## 2. Headline Features: Detailed Breakdown

This release focuses on three primary headline features, with a strong fourth supporting feature.

### A. Task Timeline Visualization
*   **User Benefit:**
    *   Provides unprecedented transparency into Cline's "thought process," allowing users to intuitively understand the *story* of how tasks are accomplished, both during and after task completion.
    *   Offers a better sense of patterns in how users interact with Cline.
    *   Facilitates retrospective analysis and learning.
*   **Wow Factor/Unique Aspect:**
    *   Visually compelling and innovative way to represent agentic work.
    *   A foundational step towards future multi-agent orchestration, offering a glimpse into how complex agent interactions will be visualized and understood.
    *   Sets a new standard for transparency in AI coding tools.
*   **Connection to Cline's Core Positioning (White Paper):**
    *   Directly manifests Cline's commitment to "absolute visibility" and "radical, real-time visibility into all agent actions."
    *   Reinforces the "true human-in-the-loop experience."
*   **Visuals:** `[VIDEO: Task Timeline Demo]` / `[VISUAL: Task Timeline Screenshot - showing hover preview]` / `[VISUAL: Conceptual slide on multi-agent timeline inspiration]`

### B. Gemini 2.5 Pro Implicit Caching Integration
*   **User Benefit:**
    *   Delivers significant cost savings for users of Gemini 2.5 Pro without requiring any manual configuration.
    *   Makes leveraging powerful frontier models more affordable and efficient.
*   **Wow Factor/Unique Aspect:**
    *   Seamless, automatic cost reduction.
    *   Highlights Cline's proactive collaboration with model providers (Google) to enhance user experience and value.
*   **Connection to Cline's Core Positioning (White Paper):**
    *   Demonstrates "unfettered access to AI models" and Cline's commitment to not just providing access but optimizing the ecosystem around it.
    *   Aligns with "abstains from the inference margin game," focusing on user benefit.
*   **Visuals:** `[VISUAL: Cache UI indication for Gemini if applicable, or conceptual graphic]`
*   **Note:** Mention Google's feedback reception and the positive impact. Plan to quote-tweet Google's announcement about implicit caching.

### C. Revamped Community-Friendly Documentation (Mintlify & In-Repo)
*   **User Benefit:**
    *   Significantly lowers the barrier for community contributions to Cline's documentation.
    *   Makes documentation more accessible, up-to-date, and easier to navigate.
    *   Fosters a more collaborative and transparent development ecosystem.
*   **Wow Factor/Unique Aspect:**
    *   Directly empowers the community to shape and improve a critical resource.
    *   Moves docs from a private, separate repo to a public, integrated part of the main Cline repository.
*   **Connection to Cline's Core Positioning (White Paper):**
    *   Embodies the "open-source ethos" and the belief in "community's collective intelligence."
    *   Reinforces Cline as a platform "powered by our community."
*   **Visuals:** `[VISUAL: Screenshot of new Mintlify docs interface]` / `[VISUAL: Example of an easy documentation contribution on GitHub]`

### D. Enhanced Editing Workflow (Non-Blocking UI) - *Prominent Supporting Feature*
*   **User Benefit:**
    *   Users are no longer "stilted by Cline" or locked out while Cline is editing files.
    *   Ability to type the next message, scroll, and click around maintains development flow and significantly reduces friction.
    *   Makes the interaction with Cline feel smoother, more responsive, and less intrusive.
*   **Wow Factor/Unique Aspect:**
    *   The tangible feeling of uninterrupted workflow and responsiveness.
    *   Cline works in the background without "stealing focus."
*   **Connection to Cline's Core Positioning (White Paper):**
    *   Directly enhances the "agentic coding experience" by making Cline a more seamless partner.
    *   Aligns with the vision of an AI that "augments human ingenuity" without causing frustration.
*   **Visuals:** `[VIDEO: Demo of Non-Blocking UI - showing typing/scrolling while Cline edits]`

## 3. Supporting Features & Quality-of-Life (QoL) Updates

These will be detailed in the "And More..." section of the blog, and used for Discord/Twitter.

*   **Quote Previous Message in Chat:**
    *   **Benefit:** Allows for more granular feedback and clearer contextual conversations, especially during planning. Enhances collaborative feel. This feature was driven by internal insights (e.g., from engineer Ara, @arafatkatze) on how pinpointed interactions lead to better results with Cline.
    *   **Visual:** `[VISUAL: Screenshot of Quoting Message in Chat]` / `[VIDEO: Demo of quote message for better plan feedback]`
*   **Larger File Analysis Support:**
    *   **Benefit:** Cline can now ingest and analyze much larger individual files, unlocking the full potential of large context window models (e.g., Gemini 2.5 Pro). No more artificial restrictions.
    *   **Visual:** `[VISUAL: Conceptual graphic of large file being processed]`
*   **Improved Terminal Command Stability:**
    *   **Benefit:** Significantly reduces instances of terminal commands freezing or locking users out of tasks. Makes Cline feel more reliable and robust.
    *   **Visual:** (Perhaps a before/after conceptual or just text)
*   **Simplified Home Header:**
    *   **Benefit:** Provides a cleaner, more professional, and sleeker first impression and user interface.
    *   **Visual:** `[VISUAL: Screenshot of Simplified Home Header]`
*   **Copy Buttons (Task Header, Assistant Messages, Code Blocks, Markdown):**
    *   **Benefit:** Simple convenience for faster reuse of information and code snippets. (Thanks **@weshoke** for markdown button in 3.14, expanded here!)
    *   **Visual:** `[VISUAL: Screenshot of new Copy Buttons]`
*   **Favorite Tasks:**
    *   **Benefit:** Allows users to preserve important or ongoing tasks when clearing history, treating tasks like persistent stories or workspaces.
    *   **Visual:** `[VISUAL: Screenshot of Favorite Tasks feature]`
*   **Generate Commit Message via Cline (Thanks @zapp88!):**
    *   **Benefit:** Streamlines a common developer task using Cline's contextual understanding.
    *   **Visual:** `[VISUAL: Demo/Screenshot of Commit Message Generation]`
*   **UI for Windsurf and Cursor Rules:**
    *   **Benefit:** More seamless experience for users in Cursor and Windsurf environments, as Cline will now use their existing rules without duplication.
    *   **Visual:** `[VISUAL: Screenshot of Windsurf/Cursor Rules UI in Cline]`
*   **UI Update for Auto-Approve (with "Approve All Commands" button):**
    *   **Benefit:** More sleek and intuitive UI for managing auto-approve settings. The "Approve All Commands" button is a significant UX win for power users.
    *   **Visual:** `[VISUAL: Screenshot of new Auto-Approve UI with 'Approve All' button]`
*   **Report Bug Slash Command:**
    *   **Benefit:** Streamlines bug reporting by allowing users to create issues with contextual information directly from the chat. Empowers the community to help improve Cline.
    *   **Visual:** `[VISUAL: Screenshot of /reportbug command in action]`
*   **Batch Selection and Deletion of Tasks in History (Thanks @danix800!):**
    *   **Benefit:** More efficient management of task history.
    *   **Visual:** `[VISUAL: Demo of Batch History Deletion]`
*   **Other Changelog Items:**
    *   Add cache to UI for OpenAI provider (related to Gemini caching transparency efforts).
    *   Add FeatureFlagProvider service for Node.js extension side.
    *   Add npm script for issue creation (Thanks @DaveFres!).
    *   Add confirmation dialog to Delete All History button.
    *   Add Mistral Medium-3 model.
    *   Add option to collect events to send them in a bundle.
    *   Update change suggested models.
    *   Update fetch cache details from generation endpoint.
    *   Update `isOminiModel` to include `o4-mini` (Thanks @PeterDaveHello!).
    *   Update defaults for Bedrock API models (Thanks @Watany!).
    *   Update to extend ReasoningEffort to non-o3-mini models (Thanks @PeterDaveHello!).
    *   Update to give error for images larger than 7500x7500.
    *   Update announcement so previous updates are in a dropdown.
    *   Fix for markdown copy excessively escaping characters (Thanks @weshoke!).
    *   Fix for loading issue with application inference profile (Thanks @WinterYukky!).

## 4. Content Plan per Asset (Ref: `.clinerules/release-content-generator.md`)

**General Notes:**
*   **Tone:** Enthusiastic, informative, user-benefit focused, aligned with Cline's positioning (powerful, transparent, community-driven).
*   **Visuals:** All `[VISUAL: ...]` and `[VIDEO: ...]` placeholders to be reviewed and assets sourced/created by the user.
*   **Pro-Tips:** To be identified and drafted collaboratively once the main content is fleshed out.
*   **Marketplace CTAs:** Confirm which marketplaces (VS Code, Cursor, both, neither) for each asset. Default to "VS Code Marketplace" or "VS Code/Cursor Marketplace" as appropriate.

### A. Blog Post (`blogs/release-3.15.0.md` or similar)
*   **Structure (Storytelling-First Approach):**
    1.  **Title:** "Cline v3.15: Unveiling Task Timeline, Gemini Implicit Caching & New Community Docs"
    2.  **Engaging Introduction:** Set the stage with the overall theme (e.g., Cline's evolution driven by community collaboration and a relentless pursuit of a better AI coding experience). Briefly introduce that this release is packed with features born from real-world challenges and user insights.
    3.  **The Story of Our Headline Features:**
        *   **The Task Timeline: Visualizing the Agent's Journey**
            *   *Origin Story:* Discuss the strategic thinking around multi-agent orchestration, the challenge of maintaining visibility, and Nik Pash's (pashmerepat) vision.
            *   *Community Collaboration:* Highlight eomcaleb's crucial contribution in bringing the first version to life.
            *   *The "Why":* Explain the problem it solves (understanding complex agent actions, retrospective analysis, pattern recognition).
            *   *The Feature & Its Benefits:* Detail what the Task Timeline is, how it works (the "storyboard" concept), and its impact on users.
            *   `[VIDEO: Task Timeline Demo]` / `[VISUAL: Task Timeline Screenshot - showing hover preview]` / `[VISUAL: Conceptual slide on multi-agent timeline inspiration]`
        *   **Taming the Token Giant: Seamless Gemini Implicit Caching**
            *   *The Challenge:* Describe the community and internal pain points with previous Gemini 2.5 Pro caching (cost, unreliability).
            *   *Advocacy & Collaboration:* Detail Nik Pash's (pashmerepat) public feedback and Google's (Logan Kilpatrick, OfficialLoganK) responsive engagement.
            *   *The Solution & Its Impact:* Explain what Gemini Implicit Caching means for users (significant, automatic cost savings) and Cline's integration.
            *   `[VISUAL: Cache UI indication for Gemini if applicable, or conceptual graphic]` / `[VISUAL: Screenshot of Logan Kilpatrick's tweet]`
        *   **Docs by the People, for the People: Our New Community-Powered Documentation**
            *   *The "Why":* Explain the move to Mintlify and in-repo docs – fostering transparency, enabling easier contributions, keeping docs fresh.
            *   *Empowering the Community:* Emphasize how this opens the door for users to directly shape this vital resource.
            *   *The Feature & Its Benefits:* Showcase the new platform and its advantages.
            *   `[VISUAL: Screenshot of new Mintlify docs interface]` / `[VISUAL: Example of an easy documentation contribution on GitHub]`
        *   **Staying in the Flow: The Uninterrupted Editing Experience**
            *   *The Spark:* Recount Siddharth Ahuja's (sidahuj) insightful feedback during his visit about wanting more control and less lockout during Cline's edits.
            *   *The Problem Solved:* Explain how the non-blocking UI addresses this, allowing users to continue working.
            *   *The Feature & Its Benefits:* Detail how this improves workflow, responsiveness, and the overall feel of using Cline.
            *   `[VIDEO: Demo of Non-Blocking UI - showing typing/scrolling while Cline edits]`
        *   *Each story section to naturally weave in: What it is, Why it matters (user benefit), How it connects to Cline's vision, `[VISUAL/VIDEO]` placeholders, and potential Pro-Tips (Cline to suggest, user to refine).*
    4.  **More Enhancements to Elevate Your Workflow (QoL Updates):** Briefly cover other important features (Quote Message with Ara's (arafatkatze) insight, Larger Files, Terminal Stability, UI updates, etc.) with concise benefits and `[VISUAL]` placeholders. Acknowledge community contributions here.
    5.  **Concluding Section:** Include standard links to full Changelog, Docs, Reddit, Discord, and Review page. (Note: User has requested to omit a direct "Update now via Marketplace" CTA for the blog post).
*   **Specific Asks from Workflow:**
    *   "Is there a specific previous release structure...?" -> Yes, emulate v3.13/v3.14 storytelling.
    *   "Should I include 'Pro Tips'?" -> Yes, Cline to suggest.
    *   "Confirm which marketplaces..." -> CTA for direct update omitted from blog; standard links remain.

### B. Reddit Post (`reddits/release-3.15.0.md` or `release-promo/3.15/reddit-post.md`)
*   **Structure:**
    1.  **Title:** Feature-driven and concise for Reddit (e.g., "Cline v3.15 is here! Featuring Task Timeline, Gemini Caching, New Community Docs, Non-Blocking UI, and more!").
    2.  **Body:**
        *   Brief intro paragraph.
        *   Bulleted list or short paragraphs summarizing the headline features and key benefits.
        *   Mention other significant QoL improvements.
        *   Include relevant `[VISUAL/VIDEO]` placeholders (or links to them if hosted).
        *   Call to action: Link to Blog Post for full details, Changelog, Discord.
*   **Specific Asks from Workflow:**
    *   "Is there a specific previous release structure...?" -> Emulate general Reddit release post style (concise, feature highlights).
    *   "Confirm which marketplaces..." -> To be confirmed.

### C. Discord Announcement (`discord-announcements/release-3.15.0.md` or `release-promo/3.15/discord-announcement.md`)
*   **Format (as per workflow):**
    ```
    v3.15.0 @everyone

    [Optional Intro Line - e.g., Packed with UX improvements and new insights!]

    [VIDEO: Release Overview (Optional Placeholder)]

    Key Highlights:
    *   **Task Timeline Visualization:** Understand the story of your tasks like never before! `[VISUAL: Task Timeline Screenshot]` (Thanks eomcaleb! 🙏)
    *   **Gemini 2.5 Pro Implicit Caching:** Save on costs seamlessly when using Gemini 2.5 Pro.
    *   **New Community Docs Platform:** Our docs are now open source and easier to contribute to! `[VISUAL: Docs Screenshot]`
    *   **Non-Blocking UI:** Keep working while Cline edits files – no more interruptions! `[VIDEO: Non-Blocking UI Demo]`
    *   **Quote Messages:** Easily reference previous messages in chat for clearer conversations. `[VISUAL: Quote Message Screenshot]`
    *   **And many more improvements!** Including better terminal stability, larger file support, UI updates for Auto-Approve & Windsurf/Cursor rules, copy buttons, favorite tasks, and a new `/reportbug` command. (Thanks zapp88, danix800, DaveFres, PeterDaveHello, Watany, weshoke, WinterYukky, and other contributors! 🙏)

    [Optional: Huge thanks to all community contributors! 🙏]

    **Update now** via VS Code/Cursor Marketplace!

    Read the full details: [Link to blog post]
    Changelog: https://github.com/cline/cline/blob/main/CHANGELOG.md
    Docs: https://docs.cline.bot (or new Mintlify URL)

    If you have a chance to support us by [leaving a review](https://marketplace.visualstudio.com/items?itemName=saoudrizwan.claude-dev), we'd greatly appreciate it. Thank you!

    [Optional closing, e.g., Happy Coding!]
    ```
*   **Specific Asks from Workflow:**
    *   "Confirm which marketplaces..." -> To be confirmed.

### D. Twitter Thread (`release-promo/3.15/twitter/thread.md`)
*   **Structure:**
    1.  **Hook Tweet:** Announce v3.15, highlight 2-3 top features, include a key visual/GIF. (e.g., "🚀 Cline v3.15 is LIVE! Get ready for the new Task Timeline, seamless Gemini Caching, and our new community-driven Docs! 🔥 [VISUAL: Montage or Task Timeline GIF]")
    2.  **Tweet 2 (Task Timeline):** Detail Task Timeline, benefit, `[VISUAL/VIDEO]`.
    3.  **Tweet 3 (Gemini Caching):** Detail Gemini Caching, benefit.
    4.  **Tweet 4 (Community Docs):** Detail New Docs, call for contributors, `[VISUAL]`.
    5.  **Tweet 5 (Non-Blocking UI):** Detail Non-Blocking UI, benefit, `[VISUAL/VIDEO]
