**Title:** Cline v3.18: Free Gemini CLI Provider & Major Claude 4 Optimizations

**Body:**

Hey everyone, Nick from Cline here.

Just pushed v3.18, which has a couple of big updates I wanted to share.

**Free Gemini 2.5 Pro via Gemini CLI**

First, we've added a new provider that lets you hook into the Gemini CLI. If you have it installed and logged in with your personal Google account, you can now use Gemini 2.5 Pro and Flash models in Cline for free (up to the 1k daily request limit). It's a really solid, cost-effective option.

**Big Performance Gains for Claude 4**

We also did a deep dive on optimizing our integration with the Claude 4 models (especially Sonnet). We've been focused on making file edits more reliable, and the results have been pretty significant.

In production, we've cut the failure rate on complex diff edits from 10% down to 6%.

[VISUAL: Chart showing diff edit failure rate dropping from 10% to 6%]

On our internal "hard mode" benchmarks, the success rate for these edits jumped from 64.4% to 84.3%.

[VISUAL: Chart showing hard mode benchmark success rate improving from 64.4% to 84.3%]

This means Cline is just more reliable with the models we now recommend as the default.

**Other Fixes:**

*   Fixed a race condition in Plan/Act mode switching.
*   Improved search/replace parsing.
*   Updated the default model to Claude 4 Sonnet.

You can grab the update from the VS Code or Cursor marketplace. Let me know if you have any questions.

Cheers.
