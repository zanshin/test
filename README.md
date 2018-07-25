# Introduction
This is a test repo to see what happens when you rename a branch after said branch has commits and
PRs associated with it.

## Steps to rename
* Rename the local branch

    git branch -m old-name new-name

* Delete the old-name remote branch and push the new-name local branch

    git push origin :old-name new-name

* Reset the upstream branch for the new-name branch

    git push origin -u new-name
