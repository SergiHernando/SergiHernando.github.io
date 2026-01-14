# My Personal CTO Playbook (That I Wish I Had When I Started)

> May contain traces of AI

I've sometimes asked myself: what is my method? I always answered: it depends on the context. The truth is, that's not quite right. The path I'll take does depend on the context, but my approach to problems or constraints follows certain patterns I've repeated in every situation.

Based on my experience leading technology at startup ventures in their 0 to 1 and 1 to 10 growth stages, pre-series A and post-PMF, this is the playbook I wish I had when I started in 2010 my own leadership path.

## Responsibilities

Time frame is between next year and the other next:

- **Budget**: How much money can we spend. Easy question, difficult answer. Specially difficult for leadership who's not used to make bets. They'll have a tendency to demand dates along with a list of features. I respond: What do we need to achieve in terms of business outcomes? With that I try to force a discussion with the founders so that everybody understands what should be the investment and why.

  Note to self. The 'Chief' in CTO requires two things: I control the technology budget, and I actively identify and champion new business opportunities. Without both, I'm not doing the job.

- **Teams**: Once we know the money, I can draft a plan. My plans do not include tasks, assignments nor milestones. It's a matter of hiring the right people to execute today and to be ready for next stage tomorrow. What do I look in candidates? (1) People whom I share that working software is the only measure of progress, (2) People that take nothing for granted, and (3) People that are willing to interact with other people in the organization regardless of their roles.

  A critical note: I'm building teams where there's no "yours" or "mine." Code, systems, designs — they belong to the company. People who need to satisfy individual ambitions, who need their ego stroked, who claim ownership of their work as a way to dodge accountability — those are expensive problems.

  I need people who help each other without keeping score. People who disagree but come with a proposal, not just a complaint. People who ruthlessly weight what the customer is willing to pay for, not what's technically elegant or personally interesting. People who avoid hiding behind subjectivity — "this is too hard" or "this is bad design" — and instead ask: does it solve the business problem?

  And I need people with high agency. I don't ask my direct reports to manage up; that's not their job. But when someone chooses to give me context without being asked, who cares enough to understand my decisions, who wants to be part of the leadership conversation, who pushes back when I'm cutting corners — that person multiplies my effectiveness by ten. That's the energy I'm building for.

- **Technology**: This is the obvious part, but I have to beat some intermediate monsters yet. Being the technology leader is my responsibility to research and build exactly what's important for the business to move forward. Tough but mandatory to push back engineers' ideas to implement this or that that does not clearly solves a business case. And most importantly: we must help senior engineers identify and develop those business cases.

## Heuretics

### Unwritten Rules

Every business has its own idiosyncrasies, a reason for being, or certain red lines that — especially in early stages — are not always explicitly stated verbally or in writing. One of the first things I do is identify those codes and translate them into principles that should guide my teams when in doubt.

A couple of examples. If the company is in FinTech and the product basically performs arithmetic operations with decimals, I would translate that into a team value: precision. If the product operates in a regulated environment like HealthTech, a team value would be traceability — everything we do must be recorded: when, by whom, and why.

I also keep in mind that this can change over time. I like to question the values that companies publish: talent, quality, innovation… Does anyone think you can build something without people? Or something that doesn't properly fulfill its purpose? Or that any company prefers to stagnate technologically? Of course not. Therefore, I believe values are anything but obvious. And it's impossible to describe them beforehand.

### Software

Make architectural decisions that don't limit, prevent, or constrain the company's future. Having said that: When to acquire technical debt? Do it when the the answer to these two questions is yes:

- [x] There's not enough data to make an informed decision.
- [x] If implementation must change once we get enough data, we can accommodate those changes with no major changes in the architecture.

Although business goes into software and we use software for building everything, software is just a part. For building software properly, to me it's fundamental that the following also happens:

- There's a **shared understanding** of the problems we are trying to solve among all the stakeholders.

- There's a **technical infrastructure** that has to be built. Infrastructure is not separate from the product — it is part of the product. Where your infrastructure lives and how it scales shapes what you can build and what customers can do with it.

- There are well-known **communication channels** and a **communication etiquette** in place. I try to be rigorous in how I communicate with those around me. While I greatly value informal, unstructured conversations, I need the information shared in those conversations to be preserved. Therefore, for me, both the channel and the method are important.

Depending on the objective ahead, I may need to write a lot of code just like anyone else. Even though that swallows large amounts of attention, I need to find a way to be aware of what's going on and know all the details. What do I use for that purpose?

- **Asynchronous code reviews with the scout hat on**, absolutely no intention to blame nobody. Actually, if a find a piece of code that for example does not adhere to this or that code conventions is actually my fault, not the author's.

- **Regular conversations with direct reports and peer managers**. I don't use a template to conduct 1:1 meetings and I let conversations naturally navigate recent events. Structured 1:1's give me the impression of being somewhat forced, whereas I want them to be the complete opposite.

- **Sharing in-depth periodic updates with the entire organization**.

### Working with me

I don't expect overtime. If it's happening regularly, I broke something. Occasional crunch before a major release? Fine, as long as it's the exception and everyone knows it.

On remote vs. office: I don't have a dogmatic position. Some teams thrive fully remote; others need to be in the same room, maybe especially early on when still figuring things out. IDK. For sure I'm not buying office time as a proxy for productivity: that's lazy management (to say it softly).

Creative work doesn't fit into a box. I expect the organization to be mature enough to understand this. If someone does their best thinking at 7am or 10pm, I'm not going to force them into arbitrary schedules. What I do ask for is communication. Team work only works when people actually communicate. ITOH, people should not be always available. Deep work requires protecting time.

I don't have all the answers. And more importantly: I don't want to. If you're waiting for me to tell you what to do, we have a problem. I expect you to think, propose, disagree, and own outcomes. My job is to provide context and remove blockers — not to be the repository of all decisions.

### Metrics

I'm skeptical of most engineering metrics I see companies tracking. Thinking of DORA and the like. All of that tells you nothing about whether you're moving the business forward. I want metrics to be a measure (even temporary) to improve the system itself, and for god's sake **never tied to team or individual performance**. What I do believe in: SLAs and SLOs. That is: the intersection of the commitments with ourselves and with our customers.

So, Sergi, how do you do performance appraisal? I don't. Career paths, to my understanding, must be defined around the problems and challenges people face and whether they are successful in dealing with them or not.

### Communication

Every week, we share the progress of our teams in a tone of momentum. Yes, even the failures. When something breaks — whether it affects customers or just us — we write a detailed postmortem: what happened, how we fixed it, what we're building to prevent it next time. I take full responsibility. You'll never see names in those documents. We're learning from the system, not blaming people.

### Decision-Making

Some decisions are mine to make; some are yours. Before we ever find ourselves in disagreement, we clarify which is which.

Big architectural decisions — major refactors, integrating new systems or tools, choosing between a quick-and-dirty solution or slow-and-well-built, rapid prototypes versus minimum viable products — these never happen alone. I talk with product managers and tech leads. We argue, we decide together.

I'm explicit about the framework: "On this, I decide but I need your input." Or: "On this, you decide; I'm here to support and communicate up." The boundaries matter.
