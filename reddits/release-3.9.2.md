# Cline v3.9.2 Release: Smarter File Handling & Model Recommendations
Happy Sunday everyone! Cline team was cooking last night. Here's what we've got for you:

**Key Updates:**

*   **Smarter File Change Detection:** Cline is now much better at noticing when you manually edit a file outside of its own actions. If you make changes while Cline is working, it will automatically re-read the file before attempting further edits. This should significantly reduce those annoying diff errors caused by Cline working with stale file content. Let us know how it feels!
*   **Recommended Models for Providers:** Cline now shows recommended models and makes it easier to switch between them -- our favorites are Claude 3.7 Sonnet, Gemini 2.5 Pro, and the new Llama 4 Maverick (which has also been added to Cline along with Llama 4 Scout).

**Other Improvements & Fixes:**

*   Improved file mention searching for faster results.
*   Added relevance scoring to file mentions to better sort and filter search results.
*   Added support for Bytedance Doubao models (Thanks Tunixer!).
*   Fixed an issue preventing duplicate BOM characters (Thanks bamps53!).

As always, update via your VS Code extensions tab. Let us know your thoughts!
