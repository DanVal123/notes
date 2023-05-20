# Git and GitHub

I would like to find a convenient workflow that works for me when working on a project solo.  I should also probably record here the main git commands I will be using.

To clone or bring a local repo up to date:

* `git clone https://...`: Clone a repo to my local computer
* `git pull https://...`: Pull the repo from GitHub to the local repo on my compter.

To stage and commit some changes

* `git add .`: Stage all files
* `git commit -m "message"`: Commit the changes.

To create a branch and merge it back into main

* `git branch name`: Create a new branch
* `git checkout branch_name`: Move over to the branch name
* `git merge branch_name`: Merge branch_name into the current branch.

To push the changes from the local computer to GitHub

* `git push origin main`: Will update the repo on GitHub with the changes that have been made locally.



# Git

At the beginning, I had issues using the command `git push origin main`.  I was getting an error and git was neither accepting my password nor a key.  The [solution](https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git#git-credential-manager) I found consists in typing the following two commands in a terminal
```
$ brew tap microsoft/git
$ brew install --cask git-credential-manager-core
```
