---
layout: post
title: "Useful git commands"
---
Sometime back I had to work on a very old codebase. It was using Perforce as its version control system. I never had any experience in any VCS other than git till that point. After working in Perforce for 1 year we finally switched the legacy codebase to use git. It was done as a part of an overall effort to upgrade the legacy codebase's toolchain.

While working exclusively on Perforce for approx 1 year I almost forgot the best practices I had developed while working with git. It took a couple of days of experimentation and reading to finally rediscover my git best practices. This made me realize that even things like git best practices fizzle out if you are not actively using it. Therefore I decided to document these rediscovered best practices in my own words. Aim for this page is to act as a quick refresher.

A good git alias to begin with:
```
[alias]
    co = checkout
    ci = commit
    st = status
```

Below are some commands that I find useful in day-to-day work.

**git config:** Configure git

**git clone:** Clone a repo

**git init:** Initialize a project with git tracking

**git st:** Current work (branch) status

**git pull:** Pull from the remote repo

**git co -b \<branch_name\>:** Create and checkout a new branch

**git co \<branch_name\>:** Just checkout an existing branch

**git diff:** Check the changes done so far

**git add .:** Add everything to the stage

**git stash:** Locally stash some changes for now. Useful when I want to try a new small idea on a clean slate.

**git stash apply \<stash\>:** Apply stashed changes in \<stash\> to the current branch

**git push -u origin \<branch_name\>:** Push a branch and follow on remote pointed by origin

**git push:** Simply push the changes in the branch to remote upstream

**git rebase master:** Pull changes from master to the current branch

**git merge --squash \<branch_name\>:** Pull changes from branch to the current branch (typically master or main) and squash it into a single commit. This makes sure that changes from a branch are merged into master (or main) as a single commit. It helps keeping the master (or main) branch history clean.

**git rebase -i HEAD~N:** Squash N commit history into a single commit. This is a bit elaborate where we can just "pick" the first commit and "squash" the rest N - 1. 

**git log:** Log commit history. Most of the time use --oneline argument for a quick review.

**git remote -v:** Explore all the remote repo connected with this local clone. 

**git cherry-pick \<commit_sha\>:** Pick a commit and apply temporarily. Useful when I want to incorporate changes from a single commit.

**.gitignore:** Git uses this file to identify what it needs to ignore.

### References
Below are some useful links on git:
- [Git by Atlassian](https://www.atlassian.com/git)
- [Git scm](https://git-scm.com/docs)
