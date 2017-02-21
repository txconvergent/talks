# Git and Gitflow [WIP]

Rainier Ababao - to be delivered 2/21/17

**Why is version control important?**

- What is it?
	- Let's start off with a common dilemma
	- People who don't use Git might resort to "Final_report_v1.docx" etc
	- It's a way of managing changes to documents, computer programs, large websites, etc.
- Backup
- Identifiability/Traceability
- Easy to trace back contributions to individual members of a team
- Less errors as you can see the differences between the last time you committed and make sure you, for example, didn't accidentally delete anything
- Other contributors to the code can easily see the latest version of your code or know which version of your code they're working on

**What is git?**

- Linus Torvalds - a character :)
- Version control system created by the inventor of Linux intended to keep track of Linux development
- Sets it apart from other VCSs including those at other shops is that it's distributed meaning you don't need a central server
- Relevant to both CS and business students

**What git is not?**

- GitHub--that's a website that hosts source code being kept track of by git. Users of GitHub upload git repositories up to GitHub, and GitHub has a slick user interface that lets you review diffs, comment on code, and star/track/fork/clone repositories easily
- GitHub's user experience has enabled millions of developers to start hacking on open source and build platform for portfolios - really amazing
- Comparison to the Texas Convergent Portal, **Enable**

**What can you use git for?**

- Poetry, prose, short stories (maybe)
- Code, some documents
- Rollback in production

**How does git work?**

- CS majors - what kind of data structure does this look like?
- slightly technical explanation of internals - roughly it's a merkle tree, hash chain
	- Linked list of diffs identified by SHA1 hashes of those diffs
	- If that didn't make sense to you that's OK!!!
- Trivial example (pushing to git-demo master)
- Complicated example (pushing to fork of git-demo)

**Gitflow**

- A pretty standard method of maintaining projects conceived by Vincent Driessen at nvie
- Designed around the "project release"
  - Remember agile sprints?
	- **Master branch** - official release history
		- Anything in this branch should be bug-free
	- **Develop branch** - integration branch for features - anything merged into this should pass all the tests
	- **Feature branch** - branch for implementing individual features like integrating an API, implementing a login feature, etc.
	- **Release branch** - becomes a candidate to get merged into the master, or production branch
		- Makes it possible for one team to polish the current release while another team continues working on features for the next release.
	- **Hotfix/maintenance branch(es)** - if there is a bug in the master production branch, then hotfix commits would be on branches directly made off of master
- Some shops will do "continuous integration" and then "release to prod" at some frequency
- Other shops will do "continuous deployment" and "release to prod" (maybe for a small subset of users, or everyone) as soon as all the test pass
- Developers work locally and push branches to the central repo

**Conclusion**

- Code identifiability is really important - at internships I look at the `git blame` to see WHO contributed which line of code and WHEN it was contributed (yes one can trace contributions to precision) and ask them why they wrote such a thing
- Gitflow works at startups
- There are lots of different git hosting services including
	- GitHub
	- Bitbucket
	- Gitlab

**Additional resources**

- [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
- [Comparison of Git workflows](https://www.atlassian.com/git/tutorials/comparing-workflows#gitflow-workflow)
