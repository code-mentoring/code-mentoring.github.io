---
layout: page
title: FAQ
permalink: /faq/
---

Answers to common questions that come up in our Slack channels and Meetups.

### Coding Interviews

<details>
  <summary>How to prepare for the coding interview?</summary>
  
  * After learning the fundamentals of data structures and algorithms, see [How to effectively use LeetCode to prepare for interviews](https://leetcode.com/discuss/career/449135/How-to-effectively-use-LeetCode-to-prepare-for-interviews).
</details> 

### Jitsi Meet Open Source Project
<details>
  <summary>What is Jitsi Meet?</summary>
  
  * [Jitsi Meet](https://jitsi.org/jitsi-meet/) is an open source video conferencing solution built on React (web) and React Native (mobile).
</details> 

<details>
  <summary>What are the steps to get involved?</summary>
  
  * See [how to contribute to Jitsi Meet as a Developer](https://community.jitsi.org/t/how-to-how-to-contribute-to-jitsi-meet-as-a-developer/).
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
    * [Open web accessibility issues](https://github.com/jitsi/jitsi-meet/issues?q=is%3Aopen+is%3Aissue+label%3Aaccessibility+label%3Aweb)
    * [Pull Requests](https://github.com/jitsi/jitsi-meet/pulls?q=is%3Apr+label%3Aaccessibility+) (to see other dev's work)
</details>  

<details>
  <summary>What's our Slack channel for asking questions and getting help?</summary>
  
  * We use the _#jitsi-project_ channel in the code-mentoring slack workspace.
    * Join a Meetup to get an invite to our Slack workspace.
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
