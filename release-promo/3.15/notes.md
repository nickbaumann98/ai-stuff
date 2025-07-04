So the big theme for this is just like a lot of UI/UX updates and improvements. In terms of what's really notable from here, the Task Timeline visualization in tasks is really cool. That's probably the big one. It's also done by a competing community contributor, so that's really cool. I'll show you a screenshot of it. It's just really cool; it gives you a visual representation of the types of tasks that were completed. If you hover over, you can see a little preview of them, so that's cool. Copy buttons are nice for copying messages. We simplified the landing part of it. I'll give you a screenshot of that as well. Add the ability to favorite tasks, I guess that's fine. What else? Oh yeah, so I think a kind of a big thing right now is when a client is editing a file, previously it would lock out the input text box. But now, not only can you type, you can also scroll around while a client is editing a file. It basically means you don't have to wait for Cline while edits are happening. Cline is not stealing focus anymore, which is low-key very handy. It just makes the editing process smoother. It's less... you don't have to wait for Cline, if that makes sense. Also, please ask me any questions you have. Um, what else? What else is like big and notable here? You can generate a commit message via client. I don't really know if that's cool. Oh, big one. Improvements to caching to open router and client providers. Remind me to include, we want to quote tweet a certain tweet here from Google, but it's about implicit caching. This makes Gemini like so much cheaper to use. I'll have a better sense of that as I use it. Yeah, I mean, Cline, you can now use your cursor in windsurf rules, which is nice if you're using Cline within cursor or windsurf. Oh yeah, support to quote a previous message in chat, that's cool. I'll give you a screenshot of that as well. So yeah, Gemini implicit caching, that's kind of a big one. I'll get you a blog on that. There's a lot of shit here. Oh, another cool one. We converted our docs to Mintlify, and we also moved them into the Cline repo itself. So if you're a community contributor and you want to contribute docs, that's so encouraged. We updated the file size that can be read by Cline, allowing larger files, which is kind of cool. If using Gemini 2.5 million token context window, like that's kind of a big deal actually. Oh, we updated the UI for auto-approve. That's nice. There have been a lot of issues with the terminal commands locking you out of a task, and we made some significant updates there that should prevent a lot more of those errors. 


Changelog
[3.15.0]
Add Task Timeline visualization to tasks (Thanks eomcaleb!)
Add cache to ui for OpenAi provider
Add FeatureFlagProvider service for the Node.js extension side
Add copy buttons to task header and assistant messages
Add a more simplified home header was added
Add ability to favorite a task, allowing it to be kept when clearing all tasks
Add npm script for issue creation (Thanks DaveFres!)
Add confirmation dialog to Delete All History button
Add ability to allow the user to type their next message into the chat while Cline is taking action
Add ability to generate commit message via cline (Thanks zapp88!)
Add improvements to caching for gemini models on OpenRouter and Cline providers
Add improvements to allow scrolling the file being edited.
Add ui for windsurf and cursor rules
Add mistral medium-3 model
Add option to collect events to send them in a bundle to avoid sending too many events
Add support to quote a previous message in chat
Add support for Gemini Implicit Caching
Add support for batch selection and deletion of tasks in history (Thanks danix800!)
Update change suggested models
Update fetch cache details from generation endpoint
Update converted docs to Mintlify
Update the isOminiModel to include o4-mini model (Thanks PeterDaveHello!)
Update file size that can be read by Cline, allowing larger files
Update defaults for bedrock API models (Thanks Watany!)
Update to extend ReasoningEffort to non-o3-mini reasoning models for all providers (Thanks PeterDaveHello!)
Update to give error when a user tries to upload an image larger than 7500x7500 pixels
Update announcement so that previous updates are in a dropdown
Update UI for auto approve with favorited settings
Fix bug where certain terminal commands would lock you out of a task
Fix for markdown copy excessively escaping characters (Thanks weshoke!)
Fix an issue where loading never finished when using an application inference profile for the model ID (Thanks WinterYukky!)