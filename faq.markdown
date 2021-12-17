---
layout: page
title: FAQ
permalink: /faq/
---

Answers to common questions that come up in our Slack channels and Meetups.

### Jitsi Open Source Project

<details>
  <summary>What are the steps to get involved?</summary>
  
  1. Introduction to the underlying technology (React/JavaScript).
      1. [JavaScript tutorial](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)
      1. [Intro to React tutorial](https://reactjs.org/tutorial/tutorial.html#developer-tools)
      1. [Learn React for free](https://scrimba.com/learn/learnreact) (Scrimba course)
  1. Get to know the Jitsi architecture, developer's guide and GitHub repositories.
      1. [Jitsi architecture](https://jitsi.github.io/handbook/docs/architecture)
      1. [Jitsi developer guide](https://jitsi.github.io/handbook/docs/dev-guide/dev-guide-start)
      1. [Jitsi-meet GitHub repo](https://github.com/jitsi/jitsi-meet)
      1. [Jitsi Handbook GitHub repo](https://github.com/jitsi/handbook) (documentation needs contributors too)
  1. Review *Issues* filtered by [web](https://github.com/jitsi/jitsi-meet/issues?q=is%3Aopen+is%3Aissue+label%3Aweb), i.e. related to web frontend.
  1. Review *Pull Requests* filtered by [web](https://github.com/jitsi/jitsi-meet/pulls?q=is%3Aopen+is%3Apr+label%3Aweb).
  1. Join the [Jitsi community](https://community.jitsi.org/).
      1. The community forum is great for asking questions and getting help with problems.
      1. In general, reserve opening new GitHub issues for confirmed app defects.
  1. Read [CONTRIBUTING.md](https://github.com/jitsi/jitsi-meet/blob/master/CONTRIBUTING.md).
  1. Help out by working on open [Issues](https://github.com/jitsi/jitsi-meet/issues)!
      1. Don't worry if you can't find an issue to work on right now, you can still learn by looking at other peoples’ Pull Requests or just exploring the code.
</details> 

<details>
  <summary>Building the application is not supported on Windows, can I still contribute if I only have Windows?</summary>
  
  * Yes, although only Linux and MacOS are supported to build the application, Windows users just need to use [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/).
    * After setup, if your WSL has no internet connection, follow this [guide](https://docs.microsoft.com/en-us/windows/wsl/troubleshooting#bash-loses-network-connectivity-once-connected-to-a-vpn).
</details>  

<details>
  <summary>What are good first issues for new contributers?</summary>
  
  * Bug/defect issues are good first issues because the steps to reproduce the issue and the expected functionality are clearly defined. 
  * Simply looking at other peoples’ Pull Requests and exploring the code is a great way to learn.
  * [Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/What_is_accessibility) issues in Jitsi seem easy enough to understand, and it's an important concept in frontend web development.
    * [Open issues](https://github.com/jitsi/jitsi-meet/issues?q=is%3Aopen+is%3Aissue+label%3Aaccessibility+label%3Aweb)
    * [Pull Requests](https://github.com/jitsi/jitsi-meet/pulls?q=is%3Apr+label%3Aaccessibility+) (to see other dev's work)
</details>  

<details>
  <summary>What's our Slack channel for discussions and questions?</summary>
  
  * We use the #jitsi channel in the code-mentoring slack workspace.
    * Join a Meetup to get an invite to our Slack workspace.
</details>  

<details>
  <summary>What's the bi-weekly community call link?</summary>
  
  * [https://meet.jit.si/codementoring-jitsi](https://meet.jit.si/codementoring-jitsi)
</details>  

### Web Development

<details>
  <summary>Do I need to be a "Full Stack" developer?</summary>

  No. Although smaller companies and startups might require a more rounded developer, there will be many oppurtunities for you to specialise in front-end or back-end development. Follow your interest, if you love front-end development and web design then delve deeper into those areas. Or if that doesn't interest you nearly as much as writing APIs, microservices and interacting with databases, then keep learning that area instead.
  
  Either way, the fundamentals of coding, data structures and algoritms, communication and problem solving skills are the foundation to your career, whichever path you follow.
  
</details>  
  
### GIT and GitHub

<details>
  <summary>How to keep a fork repo up to date?</summary>

* Set an upstream repo:
  * `git remote add upstream MAIN_REPO_URL.git`
* Verify:
  * `git remote -v`
* Fetch changes from upstream repo:
  * `git fetch upstream`
* Merge changes into your local fork repo:
  * `git merge upstream/main`
* Update your remote fork repo on GitHub:
  * `git push`
* [More info about GitHub Forking](https://gist.github.com/Chaser324/ce0505fbed06b947d962)
</details>

<details>
  <summary>How to fetch a Pull Request for review?</summary>

* `git fetch origin pull/#/head:pr#`
  * Where `origin` is the remote repo and `#` is the PR number.
* [More info about Fetch](https://www.atlassian.com/git/tutorials/syncing/git-fetch)
</details>
