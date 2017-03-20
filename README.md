git navigate-branch
===================

Create local aliases for easy navigation along a git branch.
Could be useful for speakers or trainers that want to show step-by-step instructions yet not type everything everytime. :)

Installation
============

In order to use the git-navigate-branch script as a new subcommand with git, 
it need to be available in your PATH.

Option 1
--------

Add the `git-navigate-branch` directory to your `PATH`:

    export PATH=$PATH:~/git-navigate-branch/bin

The additional git command can be used like any other git command.

E.g. to navigate the foo branch use:

    git navigate-branch foo

To navigate the master branch:

    git navigate-branch master



Option 2
--------

Use the Makefile to copy the scripts to your `/usr/local/bin` directory.
This will also copy the man pages to the appropriate directories on your
system.

    make install

To remove the scripts and man pages run `uninstall`:

    make uninstall

Commands
========

* `git navigate-branch` -> Select a branch for navigation
* `git first` -> Go to the root commit in the selected branch
* `git prev` -> Go to the previous commit in the selected branch
* `git next` -> Go to the next commit in the selected branch
* `git last` -> Go to the last commit in the selected branch

Credits
=======

Git next & git prev aliases copied from https://coderwall.com/p/ok-iyg/git-prev-next.
Git plugin project template copied from https://bitbucket.org/ssaasen/git-pastiche.
