Cline 3.12.1 continues our push for smarter context management, with a 30% leaner system prompt that loads dynamically, plus automatic pruning of old file versions that bloat context. For you, this means a smarter and more efficient Cline. 🧵

Why this focus on context efficiency? Reducing noise – like outdated file versions or prompt sections not relevant to the current task – helps Cline stay better aligned with your immediate goal, improving the reliability of its output.

Here's how the prompt is leaner: the base is 30% smaller, and detailed instructions (like tool guides) are now loaded dynamically, only when actually needed. This cuts down on unnecessary overhead in each interaction.

Context clutter from file edits is also reduced. Cline now automatically detects multiple versions of the same file in the window and intelligently removes older copies as space gets tight, keeping the latest, most relevant version active.

This is just the beginning of our push for more intelligent context management. We're actively exploring further optimizations, such as better handling of verbose terminal output, to continue improving Cline's focus and efficiency.
