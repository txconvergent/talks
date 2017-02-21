# Git and Gitflow

Rainier Ababao

**Why is version control important?**

- What is it?
	- Let's start off with a common dilemma among students
	- "Final Report v4 final final.docx" - as technologists we can do better :)
	- It's a way of managing changes to documents, computer programs, large websites, etc.
- Backup
- Easy to tracing back contributions to individual members of a team
- Less errors as you can see the differences between the last time you committed and make sure you, for example, didn't accidentally delete anything
- Other contributors to the code can easily see the latest version of your code or know which version of your code they're working on

**What is git?**

- Developed by Linus Torvalds, the inventor of Linux, to keep track of Linux development
- Version control system
- Sets it apart from other VCSs including those at other shops is that it's distributed meaning you don't need a central server

**What git is not?**

- GitHub - that's a website that hosts source code being kept track of by git. Users of GitHub upload git repositories up to GitHub, and GitHub has a slick user interface that lets you review diffs, comment on code, and star/track/fork/clone repositories easily
- GitHub's user experience has enabled millions of developers to start hacking on open source and has become a platform for code-based portfolios as well

**What can you use git for?**

- Poetry, prose, short stories
- Code, documents
- Example: rolling back in production

**How does git work?**

- CS majors - what kind of data structure does this look like?
    - Linked list
- Slightly technical explanation of internals
    - Roughly it's a Merkle tree, linked list of hashes, might be a blockchain, etc.
	- Linked list of diffs identified by SHA1 hashes of those diffs
	- If that didn't make sense to you that's OK!!!
- Trivial example (demo: pushing to git-demo master)
- Complicated example (demo: pushing to fork of git-demo and making a PR / slick slide deck viz)

**Gitflow**

- A pretty standard method of maintaining projects conceived by Vincent Driessen
- Designed around the "project release"
  - Remember agile sprints?
	- **Master branch** - official release history
		- Anything in this branch should be bug-free
	- **Develop branch** - integration branch for features - anything merged into this should pass all the tests
	- **Feature branch** - branch for implementing individual features like integrating an API, implementing a login feature, etc.
	- **Release branch** - becomes a candidate to get merged into the master, or production branch
		- Makes it possible for one team to polish the current release while another team continues working on features for the next release.
	- **Hotfix/maintenance branch(es)** - if there is a bug in the master production branch, then hotfix commits would be on branches made directly off of master
- Some shops will do "continuous integration" and then "release to prod" at some frequency
- Other shops will do "continuous deployment" and "release to prod" (maybe for a small subset of users, or everyone) as soon as all the test pass
- Developers work locally and push branches to the central repo

**Activity**

- Make a GitHub account if you don’t have one already!
- Check out txconvergent.github.io/git-demo
- Fork it, clone it, work on it, and make a pull request
- Ben will be maintaining the repository, reviewing and accepting pull requests throughout the week
- We’ll see the final result at the next GM!

**Sites made with GitHub Pages**

- 18F
- Open source software description sites at big tech companies (Facebook, Twitter, Adobe, etc.)
- My personal site

**Conclusion**

- Code identifiability is really important (show `git blame` example)
- Gitflow works at startups
- There are lots of different git hosting services including
	- GitHub
	- Bitbucket
	- Gitlab
- Differences between these and recommendations

**Additional resources**

- [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
- [Comparison of Git workflows](https://www.atlassian.com/git/tutorials/comparing-workflows#gitflow-workflow)
