README.md
---------

# Code Mentoring Website

This repo holds files for the Code Mentoring [website](https://codementoring.co/) which brings together information about our community, meetups, projects, and recommended learning resources.

This file documents:
* How jekyll makes the website
* How to install jekyll for local development
* How to make changes to the website


How Jekyll makes website
------------------------

Jekyll generates the _site directory and contents from the following:
* index.markdown -> home landing page
* _config.yml    -> config/header/footer info
* 404.html       -> used when link files not found
* (We will add more here as we go!)

The production (live) page can be found at:
    https://codementoring.co/


Install for local development
-----------------------------

After performing the following installation you should be able to:
* view the website locally via your browser
* modify the markdown files for to update the website

Installation:
1. Install necessary packages to run jekyll
    https://jekyllrb.com/docs/installation/

2. Get jekyll and bundler:
    ```
    gem install jekyll bundler
    ```
    For more details: https://jekyllrb.com/docs/

3. Target this (local) directory for gems to install (from this dir):
    ```
    bundle config set --local path 'vendor/bundle'
    ```
4. Update the gems
    ```
    bundle update 
    ```
5. Serve the website locally
    ```
    bundle exec jekyll serve
    ```
6. View the website in your browser with url:
    localhost:4000


Making changes
--------------

If you make a change to the website:
1. Test your changes locally, ensure you didn't break anything else!
2. Commit and push to your own forked repo (see git tutorials for how this works)
3. Make a pull request on code-mentoring's github.
4. After your change has been approved, it will be merged.
   After merging you will be able to see your changes go live.


Keep your forked repo up to date
------------------------
* Set an upstream repo:
  * git remote add upstream https://github.com/code-mentoring/code-mentoring.github.io.git
* Verify:
  * git remote -v
* Fetch code-mentoring changes:
  * git fetch upstream
* Then merge them into your local:
  * git merge upstream/main
* Then update your remote fork:
  * git push

[More info about GitHub Forking](https://gist.github.com/Chaser324/ce0505fbed06b947d962)
