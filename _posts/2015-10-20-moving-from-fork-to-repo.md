---
layout: post
title: From GitHub Fork to GitHub Repo
tags: [github, tutorial]
---

So a few minutes ago I moved my website (which was originally a modified fork from Jekyll Now) to it's own repository. The process to do this isn't difficult, but it also requires one to have some time avaiable. So here is a simple guide toshow you how to do this.

Step 1
======
Requirements:

* `git` installed on your computer (run `git version` on Linux systems to verify)
* An internet connection
* A GitHub fork
* Around 15-20 minutes

What will you lose?

* Releases
* Issues
* The wiki
* Pull requests

As such, the only thing preserved is your code. This makes moving a fork to a repository only useful if you have just begun/haven't had any issues yet. Otherwise you will need to move the content manually.

Step 2
======
Have a recent version of your GitHub repo avaiable. If this is your first time with `git`, copy the clone url and run

> git clone cloneurl

If you already have a GitHub repo cloned to your computer, run this in your repo directory:

> git pull

This will verify all your commits with GitHubs.

Step 3
======
Remove your old repository.

# THIS STEP MIGHT CAUSE LOSS OF DATA, I AM NOT RESPONSIBLE FOR ANY ACCIDENTS THAT MAY OCCUR!

Do this by going to settings and into the 'Danger Zone' and removing your repository.

Step 4
======
Create a new repository.

For this step, disable the option to create a Readme and make sure that your repository name is the same as the previous repository.

Step 5
======
Run the following command to get all content back on GitHub:

> git push

`git` will ask you for your GitHub username and password. Give it those and within minutes your code will be back where it used to be, only this time on it's own repository, rather than a fork.
