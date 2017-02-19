# Agile Development

Rainier Ababao - 2/13/17

### History

**Waterfall**

- great for manufacturing industries, particularly computer chip fabrication, still used today at huge shops
- after-the-fact changes are prohibitively costly (waterfall diagram) (comparison of waterfall success vs agile success in study)

**Agile Manifesto Principles**

- Customer satisfaction by early and continuous delivery of valuable software
- Welcome changing requirements, even in late development
- Working software is delivered frequently (weeks rather than months)
- Close, daily cooperation between business people and developers
- Projects are built around motivated individuals, who should be trusted
- Face-to-face conversation is the best form of communication (co-location)
- Working software is the principal measure of progress
- Sustainable development, able to maintain a constant pace
- Continuous attention to technical excellence and good design
- Simplicity—the art of maximizing the amount of work not done—is essential
- Best architectures, requirements, and designs emerge from self-organizing teams
- Regularly, the team reflects on how to become more effective, and adjusts accordingly

(I won't go over each of these--the tl;dr is that agile prioritizes iteration, continuous delivery, constant changing of requirements.

Think FB, roughly:

- "fuck it ship it"
- "done is better than perfect"
- "move fast and break things" -> "move fast with stable infra")

**Disambiguation**

- There are lots of ways to implement "agile", not everybody does it the same.
- There's scrum, kanban, test driven development, etc. (Wikipedia categories picture)
- Agile doesn't just apply to software, it can be applied to design, marketing campaigns, etc.

### Definitions and walkthrough

- There are different types and implementations of agile geared for different timelines, products, and team dynamics.
- For instance, it might be difficult for an exclusively R&D team to abide by very short sprints since it's difficult to estimate a single "unit of research". Usually the way agile is implemented nowadays is a close mixture between scrum and kanban.

_**Question** - how many of you have participated in agile development in industry before?_

**Daily standups** - called "daily scrum" sometimes because it originated from the Scrum framework, everyone goes in a circle and answers three questions:

1. What did you do yesterday?
2. What will you do today?
3. Are there any impediments in your way?

Why stand up? Because it helps it go faster, people are itching to sit back down.

**Scrum master** - facilitates meetings, helps team reach consensus for what can be achieved in time, makes sure the daily standup doesn't take too long, follows rules, protecting the team from outside distractions, etc.

**Product owner** - understands business value of product, customers demanding features, available to development team for consultation so the team implements the features correctly (show tree swing picture to demonstrate what happens when interdisciplinary communication is not present)

**Sprint retrospective** - meeting facilitated by scrummaster, at which the team discusses the sprint that was just completed and determines what could be changed that might make the next sprint more productive

**Sprint planning** - meeting facilitated by the scrum master (incubator analogue - "architect"), a product owner (incubator analogue - "product manager"), and everyone else, who defines the work and effort necessary to meet their sprint commitment

**Product meeting** - less technical, higher-level planning that might be done every two sprints, every month, or every quarter, help define backlog

**Kanban board** - visual way to manage tasks undergoing different stages, for example (show examples of kanban boards)

(Named so as this is a thing from Kanban that is borrowed by most other types of agile, including scrum.)

The major parts should be "backlog", "to do", "in progress", "done", maybe in several lanes, like "product development", "marketing", "research". Label things with how important they might be (some Kanban schemes attach Fibonacci number "values" to issues {1 2 3 5 8} to prioritize/award points), and who they're assigned to.

**Backlog** - list of requirements that a Scrum Team maintains for a product - features, bug fixes, non-functional requirements

**User story** - high-level definition of a requirement--rule of thumb is that it has just enough information so the devs can produce a reasonable estimate of the effort required to implement it


### Real-life anecdotes

- 10-person startup in Austin
- 110-person startup in Sunnyvale
- 20-person startup in London

### Tools and conclusion

Popular tools for scrum you might use in the incubator - some of which are tied directly into our portal via links to these sites and later on, API's - include:

- Trello
- JIRA (usually used by larger companies)
- Waffle.io (has GitHub Issues integration, great for developers)
- Aha! (super visual product roadmap, great for product managers)

I _really_ encourage y'all to come talk to me after and ask questions about this - it's one of the most important things you'll learn in Convergent because it ties directly into our model and will make or break your prototype development.
