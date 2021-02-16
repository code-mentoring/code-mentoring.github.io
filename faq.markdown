---
layout: page
title: FAQ
permalink: /faq/
---

Answers to common questions that come up in the slack channel and weekly meetup

## GIT and GitHub

### How to keep a fork repo up to date?
* Set an upstream repo:</li>
  * E.g. `git remote add upstream https://github.com/code-mentoring/code-mentoring.github.io.git`
* Verify:
  * `git remote -v`
* Fetch changes from upstream repo:
  * `git fetch upstream`
* Merge changes into your local fork repo:
  * `git merge upstream/main`
* Update your remote fork repo on GitHub:
  * `git push`
* [More info about GitHub Forking](https://gist.github.com/Chaser324/ce0505fbed06b947d962)
