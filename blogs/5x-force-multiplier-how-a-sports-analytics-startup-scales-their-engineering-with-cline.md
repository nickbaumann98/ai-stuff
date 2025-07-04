# “5X Force Multiplier”: How a Sports Analytics Startup Scales Their Engineering with Cline

![Nick Baumann](/_next/image?url=https%3A%2F%2Fcline.ghost.io%2Fcontent%2Fimages%2F2025%2F01%2FProfilePicture.jpg&w=96&q=75)

Nick Baumann

March 15, 2025 • 6 min read

In the fast-paced world of sports analytics, where deadlines are dictated by game schedules and championships, engineering teams face unique challenges. For Cleat Street, a fast-growing sports analytics company launched in 2019 out of a startup lab at Columbia University, the pressure to deliver quality code with a small team meant finding creative solutions to accelerate their development process.

Now based in San Francisco with additional offices in Denver, Cleat Street has rapidly expanded their operations while maintaining a lean engineering team. I recently spoke with their Engineering Manager, Chrys Propster, about how they've integrated Cline into their workflow. What I discovered was a thoughtful, systematic approach to AI adoption that's delivering remarkable results while keeping their engineers firmly in the driver's seat.

## **The Challenge: Tight Deadlines, Limited Resources**

Founded in 2019, Cleat Street has been on a mission to become the most innovative sports analytics company in the space. As Chrys explained:

> "The deadlines are tight because we are always kind of beholden to the sports schedule. Essentially, the only week you have off during the year is MLB All-Star break. Your turnarounds are tight, your deadlines are tight. And obviously being a startup, we have a really small team."

This combination of unforgiving schedules and limited resources created a need for what they call "force multipliers" – tools that could help their existing team accomplish more without sacrificing quality.

## **The Solution: Cline as a Force Multiplier**

Cleat Street began integrating Cline into their development workflow earlier this year, starting with a cautious approach focused on documentation and testing. But as engineers gained confidence with the tool, its applications expanded dramatically.

What began as an experiment has evolved into a comprehensive system that's delivering measurable productivity gains. Chrys was unequivocal about the impact:

> "On average, it's probably a force multiplier of like 5x. Something that used to take two and a half days, I can get that in half a day."

This dramatic acceleration isn't just about getting more done faster – it's about fundamentally changing how their team approaches development tasks and what they can accomplish with their existing resources.

## **Building a Connected AI Development Ecosystem**

What makes Cleat Street's implementation particularly interesting is how they've woven Cline into their existing development tools and processes. They've built custom Model Context Protocol (MCP) integrations to connect their entire workflow, which has significantly enhanced collaboration across their engineering team.

1. **Linear Integration**: Their first priority was connecting Cline to Linear, their Agile task management system. "One of the main ones was Linear, which is our task management system, our Agile system," Chrys explained. This allows engineers to quickly access and update tasks directly through Cline, streamlining their project management and keeping everyone in sync.
2. **Notion Knowledge Base**: Perhaps most impressive is their Notion integration that serves as an evolving memory bank for their engineering knowledge. Chrys explained that they've set up a system in their .clinerules where "if you change a route anywhere in the API, it automatically ships that back up to Notion using the MCP."

This interconnected system has not only streamlined their workflow but also fostered better collaboration. By hooking up "AWS, Notion, and Linear together," they've created a knowledge ecosystem that keeps everyone on the same page and makes it easier for engineers to collaborate on complex features.

## **Real-World Applications**

Cleat Street has found several key use cases where Cline delivers exceptional value:

### **1. Codebase Modernization**

The team is currently tackling three major refactoring projects:

* Converting their JavaScript codebase to TypeScript
* Refactoring to Tailwind CSS

Chrys described their approach:

> "I have three people on the team that are doing three individual tasks like that, where one person is refactoring everything to Tailwind, the other person is doing all of TypeScript, and the third person is removing select stars from the database. I want to see how all of that context builds and then gets merged back together."

These tasks, which would normally consume significant engineering resources, are now being accelerated through Cline while maintaining code quality through careful review processes.

### **2. Documentation and Testing**

A common pain point for many engineering teams is creating comprehensive documentation and tests. At Cleat Street, they've found that having Cline handle these "salt mine tasks" frees up engineers to focus on higher-value work:

> "More documentation, testing, stuff like that. It's much easier to review those documents than to come up with them fresh, especially for some engineers that might not be their strong suit," Chrys noted.

### **3. Bridging Skill Gaps**

Perhaps most interestingly, Cleat Street has discovered that Cline can help bridge specialized skill gaps on their team:

> "It's like a gap filler for skills. So if we have the need for, say, a DevOps guy who's really versed in AWS, Cline can fill that gap. As long as I make the documentation to the AWS knowledge base, Cline can go and fill that gap. And the more it builds as AWS infrastructure goes, the better it gets. So you save a lot to your bottom line not having to hire that senior AWS architect guy."

## **The Results: Surprising ROI**

The impact on Cleat Street's productivity has been dramatic, but what might be most surprising is the economic value proposition. When asked about API costs, Chrys was candid:

> "I'd probably say about a hundred bucks every two weeks," he explained, though he noted they've "gone up to like $500 about on a two-week period" at peak usage when setting everything up.

Putting this in perspective, Chrys added: "You're talking about spending an extra $12,000 a year versus hiring five people at $150K. It's incredibly worth it."

When a single engineer's fully-loaded cost exceeds $150,000 annually, and Cline enables each team member to be 5 times more productive, the return on investment becomes staggering. The math makes a compelling case for leveraging AI tools to maximize output from an existing team.

## **Keys to Successful Implementation**

Cleat Street's approach wasn't to simply deploy Cline and hope for the best. Chrys shared valuable insights about adoption strategies that other organizations can learn from:

### **1. Start Small for Successful Adoption**

When rolling out Cline, they faced the challenge of getting engineers with different skill levels and AI familiarity to adopt a new tool. Their solution was to begin with low-risk tasks that provided immediate value:

"Everybody that's starting off, especially people that haven't used AI tools before, I'm like, 'Hey, just try starting with writing documentation. Let it save files locally, don't push it up into any of our services,'" Chrys explained. "That way, they're not actually even writing code. They're getting used to prompting and what they have to do to get Cline to act, and just getting used to the different prompting styles."

This gradual approach helped overcome initial resistance and built confidence across the team. By the time engineers moved to using Cline for code refactoring and more complex tasks, they already had a solid foundation of prompting skills.

### **2. Build a Prompting Knowledge Base**

The team quickly realized that effective prompting is the key to productivity with AI tools. They created a shared resource of prompting techniques for different scenarios:

> "We're building a prompting bank with different approaches for different tasks. How you prompt for AWS infrastructure is different from how you prompt for TypeScript refactoring or API documentation in Notion. The way you prompt is where you'll live or die with these tools."

This systematic approach to documenting effective prompts has accelerated their learning curve and ensured consistent results across the team.

### **3. Iterate for Improvement**

A critical insight from the Cleat Street team is that Cline becomes more effective with repeated similar tasks. They discovered that intentionally planning for multiple iterations leads to better outcomes:

> "When Cline is starting something brand new, it takes a certain number of iterations to get it right. With a technical specification, for example, the first attempt will have mistakes that you need to correct. By the third iteration, it's usually pretty clean and becomes self-sustaining."

This observation has helped them set realistic expectations and build iteration into their workflow.

### **4. Focus on Safety and Review**

Safety has been paramount in Cleat Street's implementation. Their engineering manager emphasized:

> "We wanted to integrate this safely because it could be a double-edged sword. The last thing you want is people just copy-pasting code without understanding it. That doesn't help them learn, and it can introduce problems into your codebase."

Their safety protocols include:

* Manual review of all AI-generated code
* Beginning with local file edits before pushing to services
* Clear guidelines about appropriate use cases
* Regular check-ins to discuss best practices

## **Looking to the Future**

As the team looks ahead, they're exploring more ambitious applications, including:

* Automating the entire product development funnel from PRDs to technical specifications
* Expanding their knowledge base to handle more specialized engineering tasks
* Integrating with more of their development tools

But their core focus remains on responsible, thoughtful integration:

> "You've got to do it safely. And right now, I don't quite have the definition of what that means. But I think every single day we're making more strides towards what does 'safely' mean."

## **Key Takeaways for Engineering Teams**

Cleat Street's experience with Cline offers valuable insights for other engineering teams considering similar implementations:

1. **Start with low-risk, high-value tasks** like documentation and testing to build confidence
2. **Create connected systems** where your AI tools integrate with your existing workflow
3. **Build a prompting knowledge base** to share effective techniques across your team
4. **Set clear safety guidelines** to ensure quality and security
5. **Measure the impact** in terms of time saved and capabilities gained

For teams facing tight deadlines and limited resources, AI tools like Cline aren't replacing engineers – they're amplifying what those engineers can accomplish, turning a small team into a much more powerful force.

---

*Ready to supercharge your engineering team’s productivity? Discover how Cline can help you scale smarter and faster.* [*Get in touch today*](https://calendly.com/d/cqxz-9rn-x9v/cline-intro?month=2025-03&ref=cline.ghost.io) *and start unlocking 5x efficiency.*
