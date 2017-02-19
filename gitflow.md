# Git and Gitflow [WIP]

Rainier Ababao - to be delivered 2/21/17

**Why is version control important?**

- Backup
- Identifiability/Traceability
- Easy to trace back contributions to individual members of a team
- Less errors
- Other contributors to the code can easily see the latest version of your code or know which version of your code they're working on

**What is git?**

- Version control system created by the inventor of Linux intended to keep track of Linux development
- Relevant to both CS and business students

**What git is not?**

- GitHub--that's just a website that hosts source code being kept track of by git. Users of GitHub upload git repositories up to GitHub

**What can you use git for?**

- Poetry, prose, short stories (maybe)
- Code, some documents

**How does git work?**

- slightly technical explanation of internals - it's a merkle tree
- Local
- Remote
- Trivial example (toy personal project example)
	```
	git add .
	git commit -m "Implemented search filter"
	git push
	~~~ do some work ~~~
	git add .
	git commit -m "Changed toolbar color from green to light green"
	git push
	```

**Gitflow**

- A pretty standard method of maintaining projects conceived by Vincent Driessen at nvie
- Designed around the "project release"
  - Remember agile sprints?
- Some shops will do "continuous integration" and then "release to prod" at some frequency
- Other shops will do "continuous deployment" and "release to prod" (maybe for a small subset of users, or everyone) as soon as all the test pass
- Developers work locally and push branches to the central repo

**Conclusion**

- Code identifiability is key
- At internships I look at the `git blame` to see WHO contributed which line of code and WHEN it was contributed (yes one can trace contributions to precision) and ask them why they wrote such a thing
- Gitflow works at startups

**Additional resources**

- [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
- [Comparison of Git workflows](https://www.atlassian.com/git/tutorials/comparing-workflows#gitflow-workflow)
