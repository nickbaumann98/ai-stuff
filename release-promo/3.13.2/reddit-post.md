# Cline v3.13.2 Patch Release: Gemini Provider Caching, Gemini 2.5 Flash Support & Community Fixes

Hey everyone,

Just pushed out Cline v3.13.2, a patch release focused on some Gemini improvements and a bunch of valuable fixes, many thanks to community contributions!

**Key Updates:**

*   **Gemini Provider Improvements:**
    *   Added caching to potentially speed things up and reduce costs.
    *   Added thinking budget support for Gemini models (Thanks monotykamary!).
    *   Added support for the new `gemini:gemini-2.5-flash-preview-04-17` model. Give it a try!
*   **Community Contributions & Fixes:**
    *   Support for `!include .file` directive in `.clineignore` (Thanks watany-dev!).
    *   Correct o1 temperature being passed to the Azure API (Thanks treeleaves30760!).
    *   Increased Ollama provider timeout for larger models (Thanks suvarchal!).
    *   Improved non-UTF-8 file handling to prevent garbled text (Thanks yt3trees!).
    *   Fixed Mermaid syntax error in documentation (Thanks tuki0918!).
    *   Browser use is now supported through any model that handles images, removing the `supportsComputerUse` restriction (Thanks arafatkatze!).
*   **Other Improvements & Fixes:**
    *   Improved slash command functionality.
    *   Better prompting for the new task tool.
    *   Fixed the "add new rule file" button.
    *   Fixed settings resetting when changing providers.
    *   Fixed missing commas in terminal outputs.
    *   Fixed terminal errors caused by non-alphanumeric outputs.
    *   Fixed auto-approve settings becoming unset.

As always, update via the VS Code/Cursor Marketplace to get the latest. Let us know if you run into anything!
