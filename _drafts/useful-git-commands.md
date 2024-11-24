---
layout: post
title: "Useful git commands"
---
Sometime back I had to work on a very old codebase. It was using Perforce as its version control system. I never had any experience in any VCS other than git till that point. After working in Perforce for 1 year we finally switched the legacy codebase to use git. It was done as a part of an overall effort to upgrade the legacy codebase toolchain.

While working on exclusively on Perforce for approx 1 year I almost forgot the best practices I had developed while working with git. It took a couple of days of experimentation and reading to finally rediscover my git best practices. This made me realize that even things like git best practices fizzle out if you are not actively using it. Therefore I decided to document these rediscovered best practices in my own words. Aim for this page is to act as a quick refresher.

A good git alias to begin with:
```
[alias]
    co = checkout
    ci = commit
    st = status
```

Below are some commands that I find useful in day-to-day work.

**git config:** Configure git

**git clone:** This is to clone a repo

**git init:** Initialize a repo

**git st:** Status

**git pull:** Pull

**git co -b \<branch_name\>:** Create and checkout a new branch

**git co \<branch_name\>:** Just checkout an existing branch

**git diff** Check the changes done so far

**git add .:** Add everything to the stage

**git stash:** Locally stash some changes for now

**git stash apply \<stash\>:** Locally stash some changes for now

**git push -u origin \<branch_name\>:** Push a branch and follow on remote

**git rebase master:** Pull changes from master to the current branch

**git merge --squash \<branch_name\>:** Pull changes from master to the current branch

**git rebase -i HEAD~N:** Rewrite N commit history

**git log:** Log commit history

**git remote:** Explore all the remote

**git cherry-pick \<commit_sha\>:** Pick a commit and apply temporarily


