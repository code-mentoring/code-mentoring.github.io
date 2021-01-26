README.md
---------

We will be creating a landing page for the group
using the Jekyll, a tool for creating webites from markdown.

This file documents:
* How jekyll makes the website
* How to install jekyll for local development
* Making changes
* Your first task/exercise.


How Jekyll makes website
------------------------

Jekyll generates the _site directory and contents from the following:
* index.markdown -> home landing page
* about.markdown -> about page
* _config.yml    -> config/header/footer info
* 404.html       -> used when link files not found
* (We will add more here as we go!)

The production (live) page can be found at:
    https://codementoring.github.io


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
2. Commit and push to your own repo (see git tutorials for how this works)
3. Make a pull request on code-mentoring's github.
4. After your change has been approved, it will be merged.
   After merging you will be able to see your changes go live.


Your first task/exercise
------------------------
Add your name the contibutors.txt file.
(This file will not change the website in any way, 
but is publicly viewable on github so you can use a pseudonym or other handle if you want)
